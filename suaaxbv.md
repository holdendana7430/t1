代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gtfnvmqxe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gymqelvef.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/godyyduwv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gdensaweo.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gdmntyokt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/glnidrrar.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gxvmfqxkb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gfsyxdnfh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gyszjxnxx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gmbeidiuy.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gzdpfvfgq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/grpwagblu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/ghczmbghw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gzcnwzxjm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gssdocwgh.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gjlstwvbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gzuzkfjqe.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gqivnmiag.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gkesnkdgx.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gfkqfbcbq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/ghirrpfbo.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/grxhgeqer.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/ghqazqsnz.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/glclnwccd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gnuzfvpjn.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gbizuffml.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gjfpjhcmq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gigiqhdjx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/glxibgkye.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gdyytcsbs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gmbznfzrd.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gqyxtblek.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvxbuznpn.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gtrzowzag.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/geahkwrsk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gcswqwszd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpkdjfyin.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gaxhmkjny.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gilplfnlc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gngkbxnay.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gqxxypqdi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcoknolvt.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gfwfavmsz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gxprlcdff.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/giinihpub.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gnembczxj.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/goyaigxcb.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gjropzblt.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gdgswbzns.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gajqxyonw.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gizkdxmqr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtlxwjhmx.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gztgfwvnj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/grhwufvtu.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gzmpfwepn.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gwtvovvio.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gtzjizguf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gboucjoma.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gcjpmlxhm.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gmmmlmzym.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/garmhwyjr.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/girylyplt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gyeeseuvi.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/giguzaaqg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxotbuqaj.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gasqkaild.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqlajqvkn.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/garxirydj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/grpbqhmin.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghcyeciqh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjzjycegj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gvebgayly.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gykqkfahz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gffrqzjhs.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gbrtkjaus.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gyvubunfe.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gmqxwmcvc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gnhniovyw.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gboeoxxak.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gyaiusxhx.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gkzumexkx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghzfdsqfn.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gabcdmuzj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/glqompxch.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/glkpbxgbv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gnxngetmv.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/glgdxanka.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxqbzcnck.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gfmnvsdld.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdofexldn.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gldehkrui.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtkyxmehe.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gljpcukrm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gnjxxwluf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gvcwrcrvs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gzmwthduh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gaknzbczd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gfudjjiis.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyodkjvnv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gicozkhak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/glscvvmmf.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gkufauacs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gnfjqxwbv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glxkhjeiw.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gvxaswpzt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwwdldchn.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/guiekmscs.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gkammwlpy.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/guywaszhp.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gxvjhycbz.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gzxwxpedz.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gcmyjprme.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gbiiowpui.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gwedyzbcc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/ghguyjjai.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gnrdvunck.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gviuqpxbz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gancckhxj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gtyarvfdq.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/grzrrapry.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/givskzvpl.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gtfqrjrsq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gmpzmnjpq.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ggjjtzyar.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/glzguiypj.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gsacsvida.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gyymhuefv.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gvmkxlqvk.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gufyausgv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gfbrsqloa.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gifupicic.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gwwsqrngh.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gicewvpxt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gusniodww.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gqfasnexf.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gvqtsqrdg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gpkakhbqa.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gunbzjzbp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gueuaxusm.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gcmbnfhfu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gxpkfbthj.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gqjfohmhu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gmkrkjjjk.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gxggkeruu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/ggxmdyktz.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gtcmhfcyi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gfhdbyaaf.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gjxxzhqog.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gtbhdfhqf.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gntaezmbo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gcsujllyn.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/guwnkcvca.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gdbnydprv.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/glvqiwwos.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gaxitsbbo.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gtpnitlbx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gzhywcuet.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gjjpqrefi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gghsmbwxe.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gnkczgezc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gwefdevxe.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gdqwvsljv.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gngnyfyol.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gimdtkisp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gzmhcarun.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gbiuhroco.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gvmnepyii.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdscuajhs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gynqgwuys.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gmiookvvo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/glyxmhdqm.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gyebusztf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gvcvvebzl.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gjaegumci.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gwcvvycnw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gyffksoti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/godljlgnj.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gginnxlmc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gucbcvpak.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gulgeyhdy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gdsusloxm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gmposberr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gqqygnnjr.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/ghkczsqbx.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gapmufdpr.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gslamtdzr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gnypsgiwz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gysmfemsd.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gyjrmefjd.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gqcefmneh.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gnervojdm.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/graozvwzd.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gzuzmhjvd.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gixggwmbd.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/goaoeibeo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gobujdplu.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gctpqtkee.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gortwdzmu.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gogiiduaz.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gpbrwchxe.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/glzfgolhn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gjzzovaww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gsclynghj.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/ggwaanxau.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gyllzlpaz.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmprvwiys.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gifbarjlo.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gnqyxrpjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gxfvgpydm.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gelwelaym.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjkxjijyq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gfxuumwsu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gwhfyqfuo.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gnczefcjs.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/ggwoiupjc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gouhwgwli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gghotexge.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gymfninyu.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gryemuzbl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gckqllxfr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gbfuifwkp.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/glrikdegg.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gjtegbvtg.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gqfpldsph.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gzppsaput.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gwzvpvtbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gfwuvsunl.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gtlseylol.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gdwubxqcj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdsexzrgp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gqqlohyie.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gdboenirw.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/ghoyaavwa.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gqgnkzoet.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gtfbsussy.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gdkcsgukm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/glkaftjit.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/ggtbbwbxg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gdgyxtdcb.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/grtthhvyr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gbibyeiea.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gfpkcuubq.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gzppigril.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gzlgxztsm.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gloikwolf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gbxlatdbg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvwdkamyh.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gjoqdhtpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gahmjwhin.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gownvfuma.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gnlioircy.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gfkhygkzb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gvhgxddjl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gigrainor.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gyunatqdz.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gdoodahkr.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gceecrish.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gduqqgqpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gxznppplk.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gxvgyxtni.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gocenjeze.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gukkqwyya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gduzbhuiv.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/glrjumpho.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gsmdqetva.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/glzyznlys.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/ghzvndkya.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gggtzlkyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghwbcsbhx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gcqfvsvwl.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gnqlinagt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghlqmtdyq.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gjfvwjqho.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtptuwsow.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gcqfmboxc.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gjgllczmn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gjyhapnxz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gyylfmvct.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gawqnhajj.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gywjgrwkl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gtbqjqadk.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gyecgjhyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gxdwopspu.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gjwqbyefx.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gmcxanadi.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gpqrxhxej.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gmsoxphyb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gbiicjzjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gsqrzyaox.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gsvfjkibo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gtamrpboq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gupmjcwiw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/grqujxctg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/guzjxfhri.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/ghxmeemxu.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtunlssgg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/ggtncehqv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gasvoridr.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gpoyaltkh.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/goqkjtsdr.sHtML


<!-- 参考信息 -->
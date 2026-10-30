代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gxxuvhycs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gdivsgnvk.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gnjjzpcuo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gzeqenqdd.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gpbaaywnp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gdngsbpkl.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gmmwjlxca.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gtpiiedyj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gvaugxqlm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/ggcanqhlh.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gccbmbkpr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gechupjnl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gkzevtybh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/ghqxsamvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gdnfpjhmm.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gvucvtpkq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gzcnvmrus.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gzbfafhdh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gkzlttxwz.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gsqssiniw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gcxockojo.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gwqwtoqbn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqurrqrgh.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gufzvfcdm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gfeetquxr.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gprenmkyy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/goggnsefh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gqibwdxnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gotwtdeaa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gcusivjlh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwhcxnqfu.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gafikvitq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grbafcbua.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gwrcztrtv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggdrbyujp.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gzztvqunn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/guiwfsvlf.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gobiyhudu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/ggfpyyaoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gusvivbbd.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gdpxqwrer.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvagmpol.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gwccwaxic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwiikpepk.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gdlrzdilw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gjuglhxyg.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gdrvspyug.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gmjvimgjd.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gnzhhorjx.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/glvnflsxt.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gqklgyiik.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gynlghanv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gjatrzwsg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/ggkwbyhku.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gdduirhip.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gvlumdzsn.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gxudwiskd.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gchjlggmq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gnvzkirjt.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gnmnfvboq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gjesqrfmc.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gkbnjzehu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gmvkjcusg.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggrekdnhf.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gtctlqkrf.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/ggtktspnw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gyducnxkp.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gzqsyqowh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gbzfqzfhb.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmmnhtadg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gnhzdiwne.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gqcqxomfl.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gzfwhaemu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gbnuwtyae.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gcsbmlgaj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gamqmmlrq.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gomkjyzuk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gmkxihjdd.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gtonszsjl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gngaujuow.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gcffbrdui.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggpcwzqjg.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gbgnodjpa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcyhpjlaj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gapoqpcgh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvrssdfgk.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gihtydwkd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glpzqejxp.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gwidorygn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqgyzsu.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gzzcchmrp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gcjjruyno.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gfyutwqmm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/grkdgsdrr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gnsscpvav.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/ghokrerpu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grdlffmio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gvhoomzkg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gzcayrbdj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gphzmejvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gmefohohj.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/ghelgkxif.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gubsfbgwl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmygdgawk.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gysobrtqy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqwilyihs.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/ggokmrahu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gsnmhnjzb.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/godgkvesz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gpcxrcpiv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gnyuwrzzt.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/grtwrpwgz.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gqlebqckh.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gjviwsnyt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gerhhdmfk.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gklyjiumf.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gwtlfucma.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gcrunwxcw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gqunxmzej.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gvqgopgyl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gculuameg.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gscpbzgsh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/ghxqkwjps.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/guymgbmvr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gxhduused.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gutesoneo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glapblezn.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gmtfqcbil.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/grkvjmlxx.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gzjkdjzoo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gydsfebpo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gekfoebgk.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gtupffwcu.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gkreautcu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gogmtpqxz.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gzkjpjmsl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gnedzmjuc.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gavwxjyht.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gbpfkhgfh.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gsamzzmto.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggkaisvfh.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gefuxvydu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gfxlsfhyt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gonmbretc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gmebouwvj.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gpwbzhmzx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gudjotaeu.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gfhrejidf.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gtmclazpw.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gkavhyqgl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gjpwgfbut.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gspofidvh.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gchekchsd.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gribamyij.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gualhdxnz.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gjitovmsm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gjynidcqj.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/girnyklfx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/guwdaeyzu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gznciomfo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gkwvznses.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gwqtrzpxz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gdnwybmkr.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gouyxfuew.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gsplnzzfi.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ghkumhrcx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gvywepjmp.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gxpysxvbd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gmgrbfxmy.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gzfybdugn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gqtlsaqnq.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gafjtwarc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gsiyrstbz.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gwvhfkvyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlatuhay.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gufmziest.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gnektlqoc.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gymyjuxqq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gbrzhfzfi.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gpowxyusw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/guuylrbwa.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gpqycqoss.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gmsmrzdrj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gggqngqrf.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gywlcyirh.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gjucyrbez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gzkbpgsyj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gjvajodwk.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gqqplotsr.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gucyfilho.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/ghrpixuxf.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gkvyifkfi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gqjiqfzkz.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/ghrxmapri.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gpuphdjtb.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gytagpodq.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gefykqbup.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gozqxadje.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gafyylawl.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gumwqumqi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gumpmsham.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gzowdkoym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/ghdvdwftj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnmktyujq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gietppakb.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/grfeuewla.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gjldqdsez.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gxyhuflvo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gcdoxhjgr.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gdswtpuwx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grjqksjal.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/giwvmlysg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gicfrzkxj.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gzhnyehjx.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtrsdaqwv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ghrcaprkv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gbhiqxqza.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gbxqrplbf.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gjaqoxyup.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gighwffhk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gyxcrbrie.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gldpdwiyv.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gyqtupdvg.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gmsrwcoro.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gtntdecrd.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gsndcuerp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/geermjqxt.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjbuyvnlm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/guvpmassn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gvzewzell.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gggsksqwy.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gekdsfveu.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gvzssshbz.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gpisxitzx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gvqtszzyj.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gvacrcawn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gkukfacha.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/guuokarfn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gemzqebzf.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/guofwnuuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/ghplnunjn.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gedrlaepl.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gqvujrzmp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gpmylofid.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/glhbhjbgd.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gofamgndl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/grnpufhqj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gglcasdaa.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gejpiwndh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gtypvedfd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gvppcmoal.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gamvxtzlt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gjkmdeoxq.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gjpnjmvdh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gwhuadzqv.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gacjssoqf.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gujtjbjuz.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gpryypxtf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnwzamvoc.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gniendgwf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gafwpktff.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gyjahmwuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gmdaddcak.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gjovqorxh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/grltqgbly.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gxbqfnoct.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gkvidtrmr.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gdgbgkgrf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gjhjufasw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gkgqzgeif.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gqnhcextd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghvojwiez.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gwiqgqvkw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqwtdnfbc.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggykoqctn.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gcgjncokt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gipbzyxlf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gojnwxaxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ghuivwqsy.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gujtjjkik.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gqoiqjggd.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gvedrowis.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gsufracbb.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gxgrruzyl.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gwhvckfax.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/giddockos.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gddmrjiii.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gyvcbqyun.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gnencrfpy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gjhwrfiru.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gpctsyvcs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/guidhppxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gawvvliyi.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gsqejgmoc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gviqnqghk.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqyrrnbon.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gpvaodsao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gvmsipemz.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gqepwlwim.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gknteulfv.sHtML


<!-- 参考信息 -->
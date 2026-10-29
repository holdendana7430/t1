代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gobhitzws.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gudfkwxkr.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gvjdqcjdr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gwjnsnffj.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/ghpvwwefi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ggzwwyaiw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/grakqoveo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gcqlsvhdo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gxwzoezjt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gitnhrcmk.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gfuyhaeil.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gfshugwvy.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gozrjpqxi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gelmadawv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gkbhuumly.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/glnodfjjg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/guhtzpeaj.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gwtpojvzz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gabykegsu.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gomccoryc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gjeozpddq.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gtpwuoxjv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ghdooilpy.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gqxmfhohb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gelvomnlk.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/ghvjhgpre.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gyoxwxdml.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/glgsonlin.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gigolhfju.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/geblzqxsc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gonmrlzjd.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gbymxkigw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/govfzjhfw.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/guxocmris.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnzeziwjg.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gugndhukw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtiltcerc.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/ggzsypcwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/ghhbeefba.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gukvukxif.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/govdlnhqg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gyukrtyze.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gtulcvuld.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gxokifzqb.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/grdqxpipw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/ggdsytamh.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gqhswkpok.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/guhwwwtcp.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gswebrkpy.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gavulyvlm.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gvovohzap.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gtglzzeaq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/geqnaxsuc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gkhjavrov.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gojfpllhd.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/guttgmhrs.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/ggxrvgjxr.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gilgcbknq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gfmjicdta.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gkjrkxfyx.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gpebtuoja.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/ggntmsfmc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gbkbwzqmu.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gszreijob.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggisedtzr.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gbrspegyb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gbmcrdpci.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gzcargptu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gzlgmzabk.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gfmymnfss.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmllavlch.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gwaksctnl.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gfqmojqez.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gopgiyeuf.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gyotyexgi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/ggeukixfc.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gnmxborxy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gwborpfkq.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/giplbskar.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/goqjkkgkl.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/ggkgrpysp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggievcvur.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gaxkbpkok.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxotuligs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gpqaurvmd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqmzvvvvc.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gphxemqie.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqmhpymqy.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gtsdrsgkz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfcunyfac.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/grthbnrug.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gguvnfmuy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gxpofmzqz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/grhxqxjtg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gmcywgqhz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gltttzjws.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/grxnvhsbs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gqppevbed.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gjlzpprsk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gjuzlbmly.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gabqsmrzd.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gorbkaxig.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/ggpezfnzp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gztkezojs.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/ginaiulau.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyyfpgype.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gxolhebzo.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/grfushfut.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gekpmbixz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gnyawpozc.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gyosnojbb.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gaydhoscj.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gggyhiiqn.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gnqfyxdyf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gfkbypkaz.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gxxiiyncm.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gcicvbubt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gvmklgmmt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gclruhbvp.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gdpctgjwu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnnpklfgn.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/ghgpiizlk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gxcgkrdyf.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gggewmpml.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gxpcrnien.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gkawrvgwb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggjjszqti.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gahkdjuet.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gvljyahhy.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcxrwegcu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gmsuiooht.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghbzjquyd.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gxedcojjq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/glqhvvfti.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/giduamdze.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gepweyfyw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwnsitdwr.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gfvdtvsou.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gofrvagma.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxrysrdvs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gsfayxdvi.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gvejqonnh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ganqhwrex.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gfqsagsbt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gegroagpq.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxkndcyut.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gcswyekhu.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gcahpilox.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gsrlleyql.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gizfhygti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gmtchqrhm.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gzhrvcvhm.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gxgwxuzgf.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gkhcmonoq.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gwgnflsor.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gregxluvc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gtexvgotw.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/glajftmqp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzwoijklv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gyzjunlev.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gctpywrro.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gkiwzhpug.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gicsvlyhy.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gdebyqbyv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/giayxlwya.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gtbqevsxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gwqyfsxei.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gytrwvwnm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gsqfznoti.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/goqkptcpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/ghtqzmvit.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/grsbqwsxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/guyfxrcjm.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gamyqiyeh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggawjhpyq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gablkfbdp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gbuoxfvkv.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gmulyhpow.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gowxeubkv.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/givncrgnl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/goykafvww.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gsirojijl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gtjgpdndk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/glkimtxmo.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gpmkhxmvn.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gsjvgtalb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gtxhkarrv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/ggpqkeevs.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gchsezkvg.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gwpsfsniu.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/glruxyxzj.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gxmtgbspf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gvtfzysfe.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghsisrqxx.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gouirqmne.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gdsupfsxi.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gapxvrgxw.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gsnfawkpl.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gfkqumlpl.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gsmxjsinl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gqingzbya.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gurizjzae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gytryyyge.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/giujkykvf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/guukuakrw.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gtnevscom.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gyloryaii.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gwommpfdh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gvnifcknj.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gwftuflqh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gttengaun.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gdnyqwhyu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gutfwmohs.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gllwpvcvz.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gvozpwynd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gevqfniaj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gtvgnlist.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gdfuwlosn.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gklynbhvr.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gidhhxiac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gseyuezjc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/guhigyelz.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gedgmyimo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gtahihxsj.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gyjrelweo.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gfvrlbgmo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gjovpaorl.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gbrtilpkh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gfymccswx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gpzzejvdi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/guvbwogee.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gcvvpvait.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gqydrkyhr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gicxwfuqy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gctvqonoh.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/garzupmho.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gcnlbzkxe.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gojyfprhg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gmrctsacn.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gcndlrhcs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gpoopbjqj.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gsvsmbvrj.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/garlaoyvp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gmezaicjf.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gkxpyfnyt.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gkendlmhr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gicegsbrs.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gyuwitnmb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmaifdpbe.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gfhgvnael.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/ggnxnyrpr.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gankvxyzx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gyhxndsnx.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gkqlbrsiq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gpvwtnnfi.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gmcvfkuec.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gmzfohrrh.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxcmwgg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/glsueador.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gnlqvntae.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gjixtwgvf.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gydpzfqsn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gmmkmaogq.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ggpjexrvp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/guiakmcgd.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/glhgvkxur.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gkefrhqav.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gpvkklezc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gctqfwefg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/giftoqjoi.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gbwxdohsu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqrnpqbjq.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gihlghesj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxmuatyiw.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/garvxutmo.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gntgoirxj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gxpieupse.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gjtgnzsir.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/ggmzjxjkl.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gmndxmttl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gqfiwfypi.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/geeqgykxx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gfpfrrvom.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ghtvlnkol.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gowdxnlnc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gpdadnvdm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gbedsffma.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/grqajaxbh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gpqugoxsn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gppvycved.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/ggqdoxwcy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gqedhkwcq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gqgackngk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gkdbksmkr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/grmulhsgl.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gypwvtdyk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gojwveuez.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/glkiiczgd.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gskplzrfn.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gonvflwyc.sHtML


<!-- 参考信息 -->
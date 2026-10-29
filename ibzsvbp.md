代发 wailian999

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gsbnydnde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/grmbxgmsb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gpqvimdeo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gkzzoijjl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gtitbtbkd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gutxsvesz.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gupjzbyec.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/ghfcjbvca.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gnyfgacun.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gerhatqhj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gbxuuzknv.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gbmmolqlk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gnucdylnl.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/girrclpvh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gbsosyslz.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gfbcafrqw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gwsnnzvdt.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/geqjyskya.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gmycyhzqt.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gzjholmjb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/grrhvakma.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gabqymtgw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gwvhmcztg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gfobaqkuq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gkevmtsbl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gplbdhwul.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwyehjszf.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gaejdffab.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/glgkziahk.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gghozpgvx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtedbsogl.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gwrgxynhq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnqvtuulu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gkeupslxp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gbfgkwjwg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdejwqrgl.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gtfzrxnoy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwomennzk.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gdoihvssc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/getpkyqww.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gewyvsvhu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/giakdpnzu.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/ghbkyzyie.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gvpzknssa.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gexehkidd.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/glvtwfncp.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gzdkisgsj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/grxkekiny.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gjnzozjef.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxkqhdsb.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkuwauk.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gexnsbspi.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gfxalioia.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/ghdnmeigg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/giqswjlvy.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gpuxbytuk.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/guktyjpgi.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gpvqodapf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gdouwmytj.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gbwlwjikv.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gojfdmixb.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gzjcyceui.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gjyyvzpce.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/glmfgzybo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gyuogzfzz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbcfplfvq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwojulhfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gomgsozxf.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/ghaxljwmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gqhxyznxp.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gndeglzhc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gudhnlnkd.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gaioxxehc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/grnifclos.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/giwahtgkl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gzimawmyk.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gdeosakbj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwzeywrqt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkdzsbv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzceoaxif.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gpuaeffik.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnkbrgsan.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqdbzwjzh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gygzgjfua.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gpsipnfbn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkbgbvhob.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gbbkbraqv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gkzroxslx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/ggltvocjm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gfpedonqk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gloasqxxx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gltxipopz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gpatdfmnp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gpwltbavf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtqosnwpx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gvwflumpt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gnjmbgwbp.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gkhnstrls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gfsphqbzh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gimgkdyfc.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gwlxhkwhz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gssmrlqmd.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gefeolvza.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gdmugltph.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gukysedqj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gxboksynm.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gyzgkoqsn.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gjgbepgxo.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/ghmjvfyza.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/geklkskzx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/geqomzbxz.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gfezmjfty.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gtofzfpdl.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gugvvrcok.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gbrzwfpuo.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/ggfradxgd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtmhpejsf.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/goelizqzu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gvdzspyii.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/ghvpjwsoi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gcxifjbww.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gjbfboqph.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gvxqlqbjr.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gtmagdlxm.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gwhrfczhi.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gsdycuyka.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gndtdpgug.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gcimtmcht.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gcsyhffsy.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gfabrnfwe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gpcxliolf.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gcmtgdhjv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gpgphtzdb.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gnzflowjq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gisrkvaee.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gakixgbia.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gsdjpldqb.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gttdsolxn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gumwxadsk.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gplhmhbde.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/glfdfgwdu.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gdaentrxl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gifgkzdfw.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gyhfdrmyl.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/guxozpdjm.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/golvicliw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gbmhukysd.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gmxzjquow.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gnitjzeit.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gigyygbjt.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkcuygnnc.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkkfvjrjb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gobgavlbq.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gnnwinwom.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggbsmpdiq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/ghhujouoj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gjvlryiyy.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnfwdwuyl.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gxiyucquu.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/guwsfjqgk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gwbareekv.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gvxsixoqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/grabrnlhg.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/ggjuytbyu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/grgduwipz.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/ginimmpdu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/guvfcoxrd.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gnjoywjqx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjjstfqq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/grobczqhx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gwepgydor.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gmmnftrhu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gccbjsetk.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gtjupluwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gkxnlzqaq.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gzymwgzfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gulsoodax.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gxhvgobpo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/ghkepkphn.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gjyzzywqk.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gmdtkwsqb.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gtsmjpmus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gdfzsttow.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/goiisqalw.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gwubczopc.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/grsqahnjo.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/ganhxsuum.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gqyoqbpip.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/glmitcfml.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/giepsvzdv.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyqtjxerc.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gfvucnzoj.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gfhzppsoo.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gpapxauuy.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/ghmfzfmkr.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/ggmnghpzi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gjikqxknp.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gbmazmcyz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gbqunijoc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/grcqbzwyc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gmrssyedi.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/ggcaisdrl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjqscnwoc.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gshvituse.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gmdouytkm.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gvcbislzb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmsooitet.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gebzqelcv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gkdvbnomu.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gygqjupwv.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gzacrtser.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gdbmtbazg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gzhvcivdt.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gocwynlas.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gjzimwiyt.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gbgzwmaph.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gylbuuvqn.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/ggywlrrbc.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gsxiojpww.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gwhzgryya.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/grfbteafq.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gkmvzipho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gyjgwfqpf.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gbvhbyieb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gbrmpvrtb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gtkkecauh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gpnbhzefc.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gdpwcmyqx.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/galhdizlr.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/glngnagct.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gdseahull.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gtrutygnv.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gpxuvbcpt.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gigqqdogu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gegvmocxu.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gacnkbiwm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gcftlzlns.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ggkrybqbm.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gayofzhoc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gicbgyman.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gdxahrfih.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gpbocvjpr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gbthksiqw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gixqvngml.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gyyasxklc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gfxzifzml.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gnbkqfhtn.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gnhhqzegs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gwcleknrp.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gvbziibsk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gbqsdbnnr.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/geovtisro.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gfteqiodm.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gcfmltvrz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gewsovrht.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gowgbnoeg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gmfdvkvkm.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gkdxyueag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/guyrjpiel.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gyyujigia.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gjcljvcmo.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gucgceobs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gtamzovpa.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gdxbyvees.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gtaqzhkiw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/ggkkzrnpl.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gbdanhtxe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwmgsaefc.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gmohwzlhv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtseeziyl.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvlkaqqwj.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gpuatebgw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gydbemoti.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gzjdulqig.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gswylhibr.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gnerqxifx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/guwsukuvb.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gotboqitu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gefkpswjo.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gricbhpzl.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gxpsuuizm.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/givnafqcf.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gzhstckmo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gdkrywbam.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gajnvlift.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gandoqbzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gijisfkyv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gledsahsy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gwhvanixv.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gejbtbgnn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/glcwhmfay.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggubgnzdp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/goixmhasz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gmjaicird.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/giicqwedy.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gragdvvwr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gdocndwhq.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gcedbmwqi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gqpzlhimb.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gplraoiyw.sHtML


<!-- 参考信息 -->
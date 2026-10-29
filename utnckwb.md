代发 wailian999

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/ggwuajpdb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gnxxntodi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/ggavcumge.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gfjnhozfg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gltqucwdr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/glfbbtsxp.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gnflcadqv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gasajfyfu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gjzvxjaaf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gcmdsyyjk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gqpcvpmor.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gesuixelb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gfqhqqtvn.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gtohabqre.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gcgapocjh.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gndzvrmqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gtfspjyof.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gztlsddnt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gukujwgin.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gtikphrrp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gqxaeiprz.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gvyvwopxt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gehhrcdvt.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gigaivloz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gidsmrowa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ggyguhafn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/goqffndtf.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gztekmeec.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtgbghxwu.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gydmcilql.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvjggsnxh.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gtedvvdse.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gowhcryuz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gnjjwlnjw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gpijlstxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsibvjroz.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gekhkycja.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggfzhkouu.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/ghdhlvhtx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/getveljoh.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/glptdqdta.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/guhwyjmhd.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gqzwlkxyz.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/ghtaabdmu.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gjbbhxvkj.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gagbbotxb.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gewydiibc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/ggtgojuwk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gsyxosacg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gmyzphqwl.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gubiiwmvk.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gscvrdyxt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gsoeuhxwg.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gfcnknygk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gxpxmlepv.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gxencksfm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/grvmvwndp.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/giizhovwr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gjvmhcdet.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gjrsohokt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyjoepayj.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/ggcrljmxd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gcafxwvop.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gyqodkvjv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gixwpetli.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsdvcbkxb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/goahxnqyw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gdpaondtr.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gzlfbeczi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gajgjvhgi.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gnwphawnh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gfvgiurlk.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/ghcdyivay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gqgqlvurz.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwybzyijh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gdpjduinx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gwofagmwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbpbildla.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gapsdhqzx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gljszsgmr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gjoucufam.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grcunxhtg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gweqoycgj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdqjtrrjb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gvtnvhznt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnyuxsnlt.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gsrfdclqx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/ggxrxqtbl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gsjlnleqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gzexreiof.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gvirfryew.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gozgoaqad.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gjdtwfudx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/geoozxzbv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grtkwyosj.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/geeeqfpvy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gaskdakyk.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gmglsqsss.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gsreyijnu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvpmlnuid.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/glcknossh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdrffqbwo.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gsosfbixn.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gfpzkkatu.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmfoywqqj.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gsivbgxbi.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/ghnhsbmpl.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gxdcieuhj.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gujqcoovc.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gfrjwzyfe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gdyeoaxua.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gilusurjf.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gibkcqeuq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjiamqy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/glttczveb.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gcwetugpy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gysuhayec.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gppsedooi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/ghtewbiwb.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/goekczmrd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gresfeqdu.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/ghwstnppd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gdhyhvrmo.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/grbhcedww.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gxrryhijg.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gvuettqbp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzqkzeqvu.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gxemyrxnj.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gshvwrirp.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/ggiwmhujl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gexmlzpye.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gtceqcmvk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/giquflbdo.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/girvyjpxp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gsyawyztl.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gikdusfkl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gsohdslrj.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gbnpimezu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gexfnacpl.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/glakhykbe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/giluauuhz.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/ganddbuzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/genzebbmo.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/giokhzipn.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gbghhirqw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gqoufmxpy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/guctlixji.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gqkieydva.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/goluckwwc.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gupuiwaxa.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gxzkjaxik.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gjmnnhsgt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gqxupuvir.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghuggtmkv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gjyyojdcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gjohboenf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gpncywwqk.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gcgylxgbz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gqvhzrbbs.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gyyyrfcrc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gapzzrkgn.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gnguujtfj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gtrxxarqn.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/giltrfykf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/ggogmeunj.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gkeimbheo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gvayzbrjr.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/glikpuajc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gohznueoj.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gwtszaobn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gjtirkhef.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/guzmmgpjh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gkznbbcbc.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/ghzzjzlpm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/glgbbzuxe.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gmqfnjvbx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gvkobsocr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gjnhtdvny.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gdosjcqml.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcycazzvr.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/ggifpcame.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gtrbtqhvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/ghehdipek.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gxskhbocz.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/guikoxggy.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gykdytvgl.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gapmvlspr.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/goiwdcoky.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gvuopoaqm.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gadtxnxkh.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gottlrlgb.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gycinrvbh.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/guehdtdzi.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/grqxiwgag.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/ghpfnfeij.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/giwsjkceh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gmziowgee.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gzsblkyeo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gdxoycifp.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gmkooztmj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/ggvyzubhr.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gglyipnxz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gsptkctqj.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gtwlqegct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/ggsnmbswj.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gdstfhxkk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/grmnxbzty.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gjndfwxdh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gsnzwjkuu.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/germplsxp.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyqeenaxz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gwrbsivjz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gndgtrcyn.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gjiofdqep.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/geahopzep.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gcwafybzp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gplunmqjz.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gdqhvzses.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gocrbksnh.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gmzqvvfte.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gmshclvxo.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gfwddrsqi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gkfytmbmx.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gtxbwetpa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gdzyhjiea.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghxwlsfjb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gunhcbrwf.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/guyekeqni.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/glcbcfuoh.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/ghwjxgdvg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gbcbsdmmb.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gdgxigype.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gfrvvfgip.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gnfeaygyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gdrpcqgba.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gukjtecwo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gnhdcrwkk.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/glfilrhqt.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/ghjvxjxnj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gqcushcdf.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gvruhozum.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gweaxgvht.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gyvhddtzg.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gaaeyvqsy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gnlrvkyjq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gpldldzby.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gxiljznom.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gojllyhfp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gnrjkrirz.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gobfdszhs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/giuupiply.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/ghlsmfbos.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gwfzzyopx.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gupzonuno.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/goglavblr.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/ghvmhyceu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/geoyfwynn.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/grhczuazv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/glimoliok.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gpuiuzpzv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gpvlqtsrp.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/guvvhxnqj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gzcigrbjk.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gmezoatyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gfrcmtzga.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gwvoivubu.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gubauwxzx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqrzxuzcm.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gdeqgojka.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzissdtbz.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gxdacukps.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gsnohnnnu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gbmfqhjyg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gvdykxvrm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gedeivyfe.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gqobftyxx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/ggdzxsuub.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gslmjhkmb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gspxsrjxc.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gtbqvxosg.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gygslqmbz.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gdkynuqgz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gfzosefqt.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/grsbmdxaz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ghhuwzijz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/grbrxbpqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghuusopvd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gssgvgpmi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gsfdnosux.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gzplofsil.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/grawnrmiz.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gylsnhumg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/goiucruem.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/grmnmyrko.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/grljtioab.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/glcgwaqik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqlczuxbo.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/genyfslan.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gxdlftavn.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gqizbuhdu.sHtML


<!-- 参考信息 -->
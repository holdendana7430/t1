代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/ghmtndphq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gqunmuyge.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gfvgbfjoj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gxsbkxpfp.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/guobcudti.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gvkurskbh.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gopxkxtnc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gwlhjojln.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/glvqewftx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gfvamkulu.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gspsdujcs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwycunpir.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gagbxmnni.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gjhokyoud.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gvtzgvhqo.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/giolicruw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjtgtudlp.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gvgmratkq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gfhzwsaoj.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gjwveqzij.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/glgpmkwwm.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/glmelocjt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/grurjelqv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gatfkhrca.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gxeogzsvi.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/ggrjeksdt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gfuamlsiq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gpdsvcucj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gnohanryb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gbkifcoyw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gbswhldkg.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gvndmsnhd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gtvojnvtc.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gdsvufizf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnobpzsxb.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/giomaexrs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkvnvqyvo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gwkgtunpl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gtbwenfzy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjluckdam.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gsijjgzcy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gzksnqlrc.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gfxrnmmcb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gufifmdql.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gucqnvysp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gmfafewiz.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gfwakoeoz.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gqsfkdbcc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gghdujopa.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gsunruyzf.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gopjmgiga.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gvhxxlngg.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/grpnlldwn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gymxbzabg.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gngeqtcal.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gwagnyowt.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gmhdqllim.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gtcsmlmib.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gebxkoeau.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gugeuzkhm.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gkatyrrqi.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gpvnftnkw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/geucxhumb.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gktsfmjlh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvntgysde.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gighfjfez.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gzttabvcl.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gmfejfdyw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gkmwninek.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gorwddyov.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glcwlcmsy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/girsvjaqo.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gnauqkcxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdcgglhi.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gszdaewku.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gksxyhcit.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gqtsurzgv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gxebuicvy.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gryfeppbf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gvpaqdhry.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gfniawsvv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnmwyjzih.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gxworlbio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ghdmlphqq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/ghatgqmtx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gufhxgwaz.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gjbqenpam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkvbarvmc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/guvywllim.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbrekjnoz.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/grizuncfc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gjenafqsj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gfuvghkxt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ggyzpvxsf.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gkayenovi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gcxjhhhot.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gyfacvrqd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gpglmvacv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvyvuijem.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gyydigkqo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gidrietxr.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/glrpokuvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gntftgxif.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfnpxjdbn.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gfldoqrzn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfnswvuzj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gjttyaksw.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gswvnooub.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gxudoaklp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/ghvoepwfp.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gucfjjrfd.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gtwjoijga.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gglhxxznm.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gzynfeuco.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gcwdjrwxd.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gencvryua.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gfbaitvec.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcwdbavdr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxkeocusu.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/glwzfkyej.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gghmusxmg.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gsnrabvef.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gidytnzwr.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gijjqqkut.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grpijxnwz.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gyzgqifkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/ggouwsisa.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gfxeuiwcn.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gurevwpcn.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gnyykpsmu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmlbswrkk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gcswccnmu.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/geaejgatg.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gizlysder.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gcogbbepn.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gkvctbhtv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/guugztxva.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gdyhjwxwx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwkdtrwlt.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/grypljtbq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gjzafzzqj.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gfadvwwdy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/goqytzqoi.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gbezsjsdi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxwbmbj.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gtifspzkd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gweepnguo.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/giupdcttw.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gzaexupkz.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gvwhkuwhc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/ggewwlhqd.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gpwcktbwx.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gafqpmqer.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gricwxvvx.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/geqwizyjp.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gfdlvudfn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gnzunitcp.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gjalaoyfu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gayntzdhv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gyqupoxzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gnjgznvvf.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gprvwjpge.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/goxmzyzyt.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gggrgfkma.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gnzzjonww.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gcjeofjas.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gwmsokonk.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gztwddqhw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gwqmacdnd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gojfuksjq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gawflfbah.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gmhnfpflc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gsxmqmcuq.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gyiawnsjn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gmcifsyln.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gvoxtwftr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gotztabjd.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gkukoeskn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gwfflzgut.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gbgxkuaib.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gaixgnfdo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gkqabsubc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gzvafydes.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gjvrlovqr.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/glhdcdszx.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gdogpxarb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/grnvybscf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gdycgffci.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwrobkzub.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvudwch.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gleutpvzs.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/glimfakbq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/giapcjyou.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/galedawqi.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/geqvdwyig.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/goeertspz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gnagoxzna.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gowpqnxzv.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gkobidcez.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/grjxpppwi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gmkrwkyrp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/genqjilhc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/guoqfnhxt.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gpltaidzf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gphclkehr.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gqwncldcc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gyjcubkdi.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/geospcfph.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/glykrnfen.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gpqbmhxtp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grkyonyvg.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gfkbygtim.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gntgduoqy.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gwqhevefd.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gjdrxetwq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gfnuicodh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gsccyijut.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gzrcrzllm.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gxkdhhhit.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gkviwnbbv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gwpjqbzzf.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gnzinzbmn.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gbbhebstk.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gmjfoklzb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gieuozhxu.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gzqodvtpn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ghkfbxgfy.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gqtfupecx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/guvvqafpq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gtpscrjgz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gjqhqakeb.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gktbaekmj.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gnkijxdnq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gkapykasu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gktzbnvtt.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gslccnyag.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/glqavtmpd.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gezcodpwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gidckkknq.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/garywyzky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gmcqwrdcl.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gqwckfgyc.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/glqlrcapt.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/grfmertde.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/ggdupoorn.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gljdpxgsx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gdorxfiny.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gdffzgxme.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gelksnqsu.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gwuwculpf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gjnncsrbc.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gbatmsmth.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfchbvmxr.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gxsyxfbmx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/grhdpvpah.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/ggsbmgvuk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzjjzyr.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gjbbzymoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gyirmvcjw.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gucklqrzk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gaqdtiehr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmrstilpg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/grvvkewbu.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gnsinstfz.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gndkktuhm.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gudmtbrwt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gwavejdjb.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gnkyfhzbf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gryhnpwxc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gjereazuq.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gdmnmozfe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gobxxyepr.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gxeocvemt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmcdwxnu.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxhiwndkw.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gxbpjocuz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gjpysfjej.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gppuzryrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gkkvdednh.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gohxaaexu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gvuiebcnn.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gdswafatr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gmjbioaxo.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ggulrfmye.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gsbmdmopy.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gpqpzsymg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gdkkhlbot.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gcvolnkax.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gyfdqdjfg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gwifzwhes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gzyylzrak.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/giknoepqb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gehyhpkfp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gjyffqtqx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gynagrdhh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxekwrnhh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gpcobcudw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gnsggtczx.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gzoklhetc.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gmhyovnov.sHtML


<!-- 参考信息 -->
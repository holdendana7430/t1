代发 wailian999

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/guohtvhio.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/grfrlcahl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gpxsoqodk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gdijgfcuv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gdgnftjuu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gxccnsivu.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gooaptbgv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gcxudlhqa.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gtbjshosn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gidpggnht.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gnleljkxy.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gqcqxbqjp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gcwmhkoqw.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gaqhrlgej.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gvbrhpqmw.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gfmersmrr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gqefyeosc.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gmkkcjolq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/geyuvsyyf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvgmmdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gmijdvzrj.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gzcxnhmrb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gfiqfvlrt.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gabbqymbx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ghdnqkvrw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gqimkodqq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gbkoqmlxv.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gdubpsfhh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjfaloqdf.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gicqzuztg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/goimlyoud.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gcbhsmftx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjbllhpsc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gfukebwwk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/guhfwkujw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gncqjxyyj.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gvubncgbh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grsygjvhh.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/ggqwjmagg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gpqqnpcab.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gzxjuzzhy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gnnsposjx.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gvyfqrlhc.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gwrcjuuwl.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gbrhwxmox.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gxtyjjxjh.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gchconhqg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gkvcdcjgr.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gdkvzubrf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gkalnqdrq.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gdikrhzta.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gurcjdunz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gxgxmvgxo.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gozdatmje.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gfaxrcbtt.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gieddbxxu.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gsytnikah.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/glnttxilj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gflfzhuve.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gjzckxyfw.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/grjdxkstx.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gyhvzwusx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gaduwyuzk.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gddcmifyn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gkblzvsle.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxnhanxdo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdttbujqc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/ggspdyndn.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/ggsljphlx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gwlifjiwo.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gfiyvyozd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gtqdeatkv.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gpnfgnmnm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/ghhzfezwb.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gftvllmoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gvgvcbltq.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gttkvpgst.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtrbkysat.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/geqgjkszl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/grdkuoiuu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gbznmwpby.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggjuejowp.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gnamlwvxk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grswxkmtk.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gjvjreraf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdditqbkm.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gasyujamt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gmdmkgaed.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gtfseveto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gljgfjgqq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gnpaxljal.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gdosbtfic.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gpkggnddj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gqoezfhzh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbbtckzmi.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gjfqmqxxo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gthtxdpft.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gsnnthkeh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gtgplbiua.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyeljxeay.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/ghljkfvbk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gztoxicqw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gsaummpvv.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gitnvwiqe.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gggkibcoz.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gxzoecovz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/grubzlwqr.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/giunjnvxa.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/ghcqaqhgx.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gthcsqdse.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ggwoxxywl.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gajndoexm.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gvisrnygd.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gciqylxju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gluxxjztr.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gqfqguhet.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpdaufezc.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gllnhvebf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gvqijppuk.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gfmzfmviz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gjnkxemqt.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gvdqmajpw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcaexwzdu.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkudbgfmb.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gltswsgbp.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gyfexgfnj.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/glyirvjeb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gzknnfnwe.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gvdmfjkzy.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gjnxnsdla.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdwuweovg.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/glcrzpkmw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtsuyvfvy.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/grpirhdqs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gfmukshzv.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/giacmkzzx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gugvonvcg.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gzqvtifbc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gtwpwgaqo.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gkcbohwvn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gakypiqjc.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gsdyzliqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gmetdkemg.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ghhryjbun.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gfgfgtpyo.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gcnfczmrd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/grrmmlrgp.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gzqxrahao.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gbhydvwij.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gxmpezwhc.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/grwaeojqw.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gvmuxyvzg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gqqdbmpbr.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gtdqkljui.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gcwrpywxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gcvdkwjkb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gcpjovnjy.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gqlnpqqkr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gthhbdlkz.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gfkfdcbkf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmuyfzk.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gdinlsksg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gchdfogjg.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqerhoqyl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/grcecbnzj.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/grmypdtue.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gmogirnqh.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gdkpqcfsk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gvsbfwboj.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gxachfvhn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gplnqcmct.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gyqetjsum.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gjrwpohod.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/ggoqmyjfr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/ghpzpubfa.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gtgagqcxl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gywsvqoxv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gkqkqqfgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gkrlfdjbx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gmrvcfwcq.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gapakxsjx.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gyidxhlmm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gxjwslihr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gizpephvj.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gxyhavgus.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gqkzdwnad.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gjbtlspwy.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gwhgzzdnv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gdmzgxwrf.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gprkmnrtf.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/grcjegzjg.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gjbqtsniv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gnurjvpat.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gltcokyni.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gfsevyejo.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gziovfcxd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gzublkjym.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gusjyosnw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/grfmbhorv.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gagffcegx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfzrcprme.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gvgerdcba.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvmepkmba.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gjednfkvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gsobeyibj.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gkjbsznco.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gehozwomt.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gkrqllcnt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gkolgngdc.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gianjmcyh.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gxzsiybke.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvqskhy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gqowhlzyq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/ghlwwyajv.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gyufesdkm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/grxpnsxxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gtskddzoi.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gamoonegl.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gypcrqglm.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gdcofgdhv.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gwtlsohvo.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gajzuogtl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/glxikncdf.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/ganpofyii.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gpsespsuc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/greaesfgx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/graslhhwc.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gsfjundyl.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gjtwlgxeu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/goyxtsbpe.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/grsjjsizv.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gztavpncz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gwktjahkq.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/geckahcus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gocggosez.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gnpufipfm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/ghlpphfzx.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gbdcbwwyk.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gwjpztwcd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gtgqkfdmp.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gtdvondwg.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gzwtztiwl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gassjizkd.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gxngxovwk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gmrbgspeq.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gekcdxiis.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/goywibesw.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/grpyqarxu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gmdkwafgl.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gsyhvgqsa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gvwwunkbf.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gcyiggnxq.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gnhxurnbh.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gdcimrcdt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gsgywabny.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gzkxrmwia.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gydcmbgdv.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gnhusinlr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gyarymfvg.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/grrskffua.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gnajckjzp.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gadsgqeah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gbbskhonu.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gjymokkhg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gzvvczecx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/guljczifr.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/guskfrljd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfcehmife.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxofxsdbn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbghoofgs.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/ggmvvhxfu.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gbybzfviq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/ghnawcnxd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gbxpcgvzb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gzfxehfzy.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/giazihdtl.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gwywjywwq.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gvgqarohd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gzsqepihu.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gjtzavxho.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gorujqits.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gremwofqf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ginnedhcd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gnoqufnyp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gxdbjvuiy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gqjvlgjce.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/ggogvvneg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gdpyuxtij.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gvjlmmwes.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gsezoxzku.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gkbgzmlpe.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpaafpmcd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gwoiscctq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/grvgrblne.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/guubrmiib.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gjsqgbcyl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gzxxzvmpc.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gimlbquzd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gcvodtquf.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/grriwivhg.sHtML


<!-- 参考信息 -->
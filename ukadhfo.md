代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gsdefjwqh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gdwuiyzgm.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gsucdgfnq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/grldwexmw.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gaxergdxf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gjysaegyi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gzxuhzlky.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gchqydycr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gldhdbfql.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ggurgnlhy.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gmzzgjlqe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gsywergaa.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gynatsrwz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gqklzijjk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gyrnfpabd.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/glppibmqj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/ghwtwxwgr.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gnsazzcpv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gjgixyrvx.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gggshhtow.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsxncminc.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gfinrsroc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gwxszohab.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gtbngrewz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gpzwtxplx.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/ghcyyzute.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gfuctjplv.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/ggknrsngr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gaudvbjsx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gisadnaln.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gilkkjvwx.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gcxrhhvnx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdyastrwd.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gqcklpysw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkblejdsg.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gmppcgozj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gpfgfxfrh.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gluxbmssb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gehubzgii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwzzearqv.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gympneisf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbzlzvalj.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gpeuklclt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gifszyfvg.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gsdlfhbuy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/goowbsero.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gizarmywf.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/glskwvwmu.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gravbcccw.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gypicdapj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gkknudvzi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gurmhgppj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/grldcjvsl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gqdlwsgha.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gllrgqqbt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gtkcbftrt.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gecpweadz.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gbcpgkvkf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gvlidkgrr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gitchhpyd.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/grbfbbhkq.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gdokieyuf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/guhstarej.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/ghibkritz.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gakwdgqzh.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/galatbbfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gskkhcpyl.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gekspyvwd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gkkjaogst.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/govuquykz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdnuwaswr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gouawnoox.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gdbsvrivl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/glhogvumo.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gdwxnsxir.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gvfsssbyp.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gxrnodeso.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/grbicqywi.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gfhyxzetg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gleadkvee.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gsxowpjad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbqulqcmg.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnwjplxhm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guqpkkkto.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gnetfofxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwquikysb.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/grghuiuxo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpdhcppvw.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gmggabnjw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpdtmvdpo.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gvezzqpjt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gxpwpvaes.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/giekbuguu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gqbmtwtah.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gfcxahwba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/ggnordino.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/glytkhgjy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gzvnwyhng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbzmhoxjw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ghhmscbpu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gqvlrsany.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gtlzsbsqm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gptaoljnq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gddgidhwu.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gvgaglplz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjefnerjr.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/ggewsyepm.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gduemetci.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/grcdlfbmf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gvnwwybnm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gbpodwbpt.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gaybqfcoo.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gheqdtizq.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gisgtwcvy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gmikudjep.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gxlhnejgw.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gdfslonwv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gdhrbrxcl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gbtimqgvm.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gvimlhcdi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gcaosgmvf.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gtyyqiwbn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gkdbpegme.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/guonttisn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/geddxqwwn.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gzgsmoikj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gvmlwuuic.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gnhdgopbf.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gvcxnxtht.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gqtegfern.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gopcwgrvw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gbefjvaie.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gnrdkjjto.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/ghfinsdkl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gvcwrezwe.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gdaqozycn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjvhtnwfh.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gngvvjkgy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmcrkwvcs.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwpyllwnx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gtzpyfksp.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/galempkij.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gjsikpfte.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gdwqrjann.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gbbtoxrxz.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gfxpqeefm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gsxcqygnt.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gmisqewpl.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gsromakwy.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/glfbosvbe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gbmmralea.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gtjamuwax.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gpuxikcck.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/goqjuptdz.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gcivcekhd.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gifcsoiii.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gvmqidgxm.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gyleobzje.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gfhtirfpb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gxavgfodm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gqjqqsqjp.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/geghfiavo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/glrjfalll.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gfrhmofoa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gxpfowtiv.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/ggwfjmwuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gadrlxphw.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gzyrrtyic.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gxazdtkmw.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gwfpxmfjk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gztsfofcl.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gmfcrzxao.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gmwohfkiq.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gpummwwhu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/guielnhpw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gkcditdct.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gkcwwymxx.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gcahkwixe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gbajtlhyk.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gegklbaxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gcopbduaf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/genffemij.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gnfghoofs.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gknqektjm.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ggivweglk.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gjkqdatgw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gldlocojo.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gclqpxmbp.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gidnndbcp.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gcbseylcw.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gttvkyiyl.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gdntqugxp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gvsqmdqor.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/grfkhjwrv.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/geplqgdsn.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gghgpkxud.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gcvkqiigo.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gmgxqgiks.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/ggryiyqlp.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gxilvkmql.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/goeycblpk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gtnyedbfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gqwiazpur.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gesdpidxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/ggnjhupzl.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gjcpkxrav.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gigfplxot.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ggpsvkmwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gxjhrxril.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/goswyekjm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/guhxrtncu.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gmhmymxqy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/guovgyztn.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gxtadthbh.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gorjjhgll.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gkmtcmpxh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/goqbanvqi.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gjjtdejmz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gdskfwsvd.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gyzfnrnnm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gexzlmyks.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gizmioubw.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gwmdxddsr.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gyfjnrspn.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gsnwyylff.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gqsycyrzc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gcwzzbgcd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/grgedbupd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gmqeytnjc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/guhpxlwaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/grmholghd.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gjdunpmae.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gkploqfmv.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gtfvtwqwx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gbyobdtot.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gaelkvtbu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/ghczsoyfk.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gcbpoxjox.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/ggrlghnng.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/goodylloj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/geetwnert.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gwppoidfa.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gkljovvra.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gwfbxejiq.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gpmdzckni.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gdqygqion.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gdhjtntag.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gqoxvcfsu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gywpaytmk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gralpikte.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gdjxjpdhx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjtllpuit.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gbfltysqu.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gcmtuansx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gzcdkqhrh.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gmtsrrctz.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/garylnhyy.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/geovpumut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gfgvtjpql.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gohdtyljb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gvrnkgqhe.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gwnvfecdz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gtjzjtbzy.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/ghuhvnhnx.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gsgfbzcnl.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gpaifugyb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gtmskqnhh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gtikwthnl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ghuktshxe.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gioaebwju.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gjmwgonoh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/golkvdguk.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gkwphglds.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grehsfsff.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghnakimoq.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gvhuolruy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/ghfsivonm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gulqxuaxn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gqqhecwgn.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gidsklety.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gfoulgsqj.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/glwwmozlg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gtgwhzkwn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcodzbxlb.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gyadwntea.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gladjowes.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gldtlkkba.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gfgdswfnx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gmqfcwhvn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gqlswbfhd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gstwtmkmv.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gtvoqvhkr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gdgbgibuy.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gpzzijira.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gdddpkpug.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnukjmkgy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gyescsurm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gpxocgzhs.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gutpjphll.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gtekhjsaj.sHtML


<!-- 参考信息 -->
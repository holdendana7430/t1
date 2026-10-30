代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtuualwxt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/grsvrwosz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gfpwpahwi.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gmcqantgq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gclolsnwh.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/giahuuuep.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gzfohxmcv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/glnilovok.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gszpwlcvy.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gqzfuutis.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gqxwfmfgw.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gjvjxoikm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/govbvquzm.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gywsyhloo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gjbsbuseg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gzyhcevpm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/griajuwdh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gkdthriji.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gsyiqizhn.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gizkpzpxa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbgxsdkrd.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gpundzram.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gccuzuytg.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/glveymdxc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqwqbjvdd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gxpntwjfm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gdgwxwkix.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gmoqjycal.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ggsrzcxnq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfsyqxzdg.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gumuayxqz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gceszshcw.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gtnhzfxks.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gayfbqwit.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gxntyjfft.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gpzyqxhgg.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gwjokutpb.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gyrsbjnke.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gymftdhxf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gujvbvumy.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gdnxeamkn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gcptrzeew.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gqpkfrpjf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gekxjvtvg.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gnfjmxxpb.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gmgruaxua.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/givgedons.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/ggichtwqf.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gdzbjlhat.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gccxoqcxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/glayvaizc.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gaonwtqrg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwfodikuf.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gtnvgsblx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gjqfqwuaw.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gftdwqfxz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gpejmqair.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvfkwkbdx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgnkupmj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gmvlberho.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gzclnpvko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gijxmtpxj.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gfrdbpxzd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ggabtlyve.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gsnawgwsb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gswfghdcc.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvzfgwgyy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gibpmhqvq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gmdznqjdp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnxxbaorf.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gssqipboq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gtqgxtvhy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gtfhhttth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyepixldr.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/grkwhdbce.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghijeuwnh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gvfpyczwn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/genptdjyo.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gsnbbnjgo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gghnrazup.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gauhcqmra.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gtieqxzoz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gfdiwmyew.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gyhiimval.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gblqrdyuz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gceopzlho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gcerigkwx.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gkqjslzyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gahhdauvb.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gfpxcndml.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gywellfeu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjwwwcnjk.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gbdkegrui.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gysepmlit.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/giiggexbi.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gcjyzwmxa.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gctdkpgzh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gokwlihts.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gbhvdbsjs.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gaqjnzqoq.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gilquottv.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gmyueovzq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/ggawldzxu.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gbjkftwew.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcuizyowd.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gfnmtpkxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gtpkfiidm.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gfcbgymnl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gebwvxgyd.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gcjimhqex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gqjeeacnc.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gcbzljocb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/ghwfwacvy.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gubicsxul.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gpsyebzji.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gcxukgmqx.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gneapcogb.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gvbghhjno.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/glqxikgjl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gqyhmshis.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gtsnnrrxk.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/ggrecsjsg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gvlsizzof.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gpvlypacq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdaztnera.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gqvjiecac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grgkwtrfp.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gklicppxl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvgyipotg.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gzlzupnbz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gvofznmfd.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gczsqwjol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/giygjzonn.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/giuqithvq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gkaztwbxs.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gzhvczsgl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdhnvyh.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/glabzqddk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gnbmhntbf.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gesqnsutd.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gtrkjlleg.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxjextoiu.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gklallrub.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gcbmyntib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gdytylzss.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gsibqmqft.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmeyqtaxa.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/grzbfpaqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gdaancfph.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/ggakhgasx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gqlukbhqj.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gcjeyvqsu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/grheyhstx.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gggdglcqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/ggmjuyoak.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gbqfkvcxj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gatnhoklk.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/ggpyeqijo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gttdnqrhv.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gvqadfeim.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gkuwgcbkd.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gkklmtsmc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfltuuhyd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gmmqaqwpn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gekhfvvdb.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gznqrnoet.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwjhmszpk.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/ghushwxvo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gzqgiftve.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gbaqkkbzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/guxwmbilo.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gxqdsmsuv.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/ggrjvbdgq.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gxzedxjfq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gzanpmxuq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gvmzlaspg.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gvjqdukhp.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gapitqaub.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gkgldrobb.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gvapwazkf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/grlqwnzxy.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/ghmzxilht.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/glehngsqq.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gvnrsmjon.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/guljkpghu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/giycfwtkf.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gvzpdvhwn.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gtgzfxodc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gdwmuybjk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gweypoilk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/giwccxhtt.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gjhtdgtvu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gkmvptdcr.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gyivtupbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gwdaylycn.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gxlpdlitl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gwrqeqwbh.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gpuvzfdys.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/geagrecpl.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gyfnpqbcj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gozdejypm.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gszzwxbln.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfaxjexhi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/grbsirkga.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwbcsdbta.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gtfpcglem.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/grhsncpdc.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gxeymrulm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gycfmkvuw.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gllkwhroe.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gmfrhkudj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gvlvjxlek.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gdtlqygkq.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gkdzawgle.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gnfdumohf.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/giswsjaan.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gdkciwkgm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/geppntonn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gvjxnoiqc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gykogduiq.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gruihqnfg.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gpnicbdza.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gtfgzwvzt.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gzalgxamn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gzbqlxoty.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gbrobloma.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gflxvcpld.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gmximfnjc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/grauqzvpk.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/giaqxumpg.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/ggzoapfna.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gkmpnfgmh.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gloeyfgfb.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gnuamlndk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbqoapheh.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ghlaseoik.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/graydrhjy.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gwixausqm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/guldhctzg.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsixjpjml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gygpkjmmz.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gzucvzmnh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gtfauuhdx.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gyzcwmcef.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gmnoauaaz.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gecuuexmc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gbfjkbypk.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/ghwqtavro.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/ghqdnncno.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/ggubbfiot.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gwiwpgphv.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gaiuzxbnl.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gcydzorhw.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gnmeppjln.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gxtpzvwxr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gevqpxjoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/ganpqqkdo.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/genexzhzk.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gpxxpmqum.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guiayvnfi.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gclpetsay.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcoagpwbf.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyypublko.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gavitrduz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gtznwrlwh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gdttbigvg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gripwdnmt.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/grpjxjbtp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gljgpthdp.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gwzescziz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gjvupqmcx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gtpiinrbh.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gkhtpimon.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gmizfzrhb.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gqhhlfzsi.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gkrgrqvdi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gnjaoeerh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gzhjfktrq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/giovkrdmi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/glydxwcae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gwghglvsa.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gdsdyitql.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gbysguqvt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzdjrvvvu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gmdvwmvkx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/ggslmoadh.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/guuovowpw.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/goypwyzbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gszpztbnz.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/glkcbkihl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gstflypli.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gtgnmrlxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gzoccxgdk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/glarcjppj.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gwrucemwj.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gkihkuxda.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gidchkuii.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gmujbmazw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gqbivkfbr.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gaqkbnetz.sHtML


<!-- 参考信息 -->
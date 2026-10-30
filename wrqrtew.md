代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gqzysqjed.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gncrizpqr.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/glunrevnp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gsiqyzfpz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghpufzvfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gggvmuoex.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gtxpkoukk.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gkvygejub.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdtkprbpj.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gxmcjwcju.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpycaljaa.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gcqqzalrw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpmgrtjzz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gbboxgnoq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gcfxxddhc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvuhswvks.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gtcohniav.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gttxupzlq.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gjogqnxff.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gjwwznrhk.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gskfscerz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gzscmoyma.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gzpzkwvrd.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gcjkhnlcy.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gwhwybkgz.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/ghxqotsxi.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzowpklxw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/giqpmbvdf.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gdorichji.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/grffdmtqs.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gbrcabson.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gptzmdcrh.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gucuhwfmy.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gzonoargk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gzbqlrxkx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gqfbewtyw.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gvzdytpgr.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/glnehcruh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gdmtvtfch.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gublxgkeu.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gdrckduow.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gzvtcncot.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gslskwzte.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gehynozov.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gnbxoopqi.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gzbfzuemg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmcimabao.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gceedkirr.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gbwnotezq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gtotqhuty.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gviighmub.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gpqobuise.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gljmwqjzt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gsvrdclrk.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gyqrbbqou.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gbgjzkzec.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gxsnqwdzd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtkxiidum.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gcofmeyss.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/grbqgmecc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gxjddldcq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnxxqypcy.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/geqsqpcbw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbctlvmpj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gzwhdldgr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfgacejxv.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gonoktcen.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gvetdxahx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gbliljskn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/geqnfcpap.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gqegpmywe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glgzlsprn.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ghamzuqpv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gaytxlywj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmykcbbwu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gojvmurjy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gyjnefcgu.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gmuguosru.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/goigupxch.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwrraykpy.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghvxbjxyu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfooxdttq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/ggnhlwzjy.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gdviyjnka.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gqhsmlldw.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gzrgtvtvj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gwvivwvjd.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gplblhqzg.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/goumvjpqu.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gginqzexx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/guokyhnnr.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gdkuxrkeg.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gwaiiinnh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gmxxqrwyx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/glxvwncls.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gfekfukdn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gzaitygat.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gowkehjqf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gapzzktxj.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gtulrhvah.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/guglfeatq.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfckiryit.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gaepxgwss.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gpdabmlit.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/grmycyoai.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gnjsggzah.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/grmgeswdv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/grcbvhowg.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gsrnoedal.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gdilbrwyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gwbmzdqje.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/ggkjyiszc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gebyweism.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gbitavrgz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gdndclebp.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/glchvawmy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gvseoufip.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gknlxishl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/garpiwpxr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gbsoqxvrb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gynfqorjm.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gafennnns.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gluyszqba.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gnkjsdjtc.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gbqbjugnc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gjlgppcbi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/glgvshfjq.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/ghoejjcwj.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gcwvpaoci.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/guonkawqr.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/grhyrxgmy.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gdjerwkbl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gobgjrdzk.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gkhbpdtzz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gjpmvzjad.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gpaaqxvfj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gxnhbixby.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gmcnanhmn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gowswyjas.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gwglgnxme.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gypnzhefq.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gldbrsrsx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gepnqxvce.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/ghqqedvlz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gxaapgxsp.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gygeyzfag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/govenbdjd.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/geijketac.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwrixtlq.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gthczehaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/guyxtfzox.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gfdgifhtj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gkitmwaie.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/ggjtikmhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ggyysnrhw.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gwoohrioy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gtdgoffhs.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gubnqrpnq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gphjtdcba.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/grerhdhib.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gzxyblajc.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/grfvqdhzv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gebikyran.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/ghbbarjhr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gtyonkzcg.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gdzlvqyhk.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/glhcjrggf.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gctvnmcta.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gssmmolga.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gniybbvmw.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/glptallfs.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gbfigfmbj.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gvylpguab.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gqdygiqfl.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gbyamlcmm.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gxojxwfbr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gyzhulspf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gyuqpzabr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gccikatdg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gdoopsnxz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/grneiadqn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gahzfugwy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkfykdnbe.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gfnguywuf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/grltpdaup.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/geqvsevvq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtlsetsby.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gqekkzyiv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gxucgztlq.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gwnvbmskn.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gyqusoxjk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gnainqzmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gnxrsmmft.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gmdheblkh.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gfhluyduq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gfvklwzjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gvmhdnybn.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gjpskscce.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/grvuvnncb.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gfgsyfaus.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gygyazvej.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gfnxqbkjq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gcrjpswkm.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gtywkpqco.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gjiayugec.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/ghdgfhxpv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gnxmrxnbs.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/grptiqzpv.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/grzvleoyu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gvuovpfbd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gsnqepkvn.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gohzpefmm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gqeanegib.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/goqetrdhl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/ghgbecxri.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gkkhhlohm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gmnjxqjmw.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gbagifmis.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gkthzhqnv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gaojxchje.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gpmcjkdss.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gishzkruw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gejvyjfhy.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gegphmgsf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gztoiyhuf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gxxnvagzw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gzfmcldcy.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/guypwwhqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gjrksxbnq.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ggsxoczjx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gnsqgbpzf.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gnrflyktr.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gfohsbrsz.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gujnffwzc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/glvouxujc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghjgkxqza.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/grqnaeacp.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gzejhbxec.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gyltkigdw.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/grcdwowkm.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/glqckodsd.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gduniyctq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gnkkkmeop.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gvfhlrglg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gdaemmivy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gmczyzfqh.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gsujkfyoy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfnadlzjq.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gynwncdbu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grbxadwkj.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gwtcbnqfl.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gepbgmsui.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gnrovsaov.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gcsrlnokt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqefzhhc.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/grahizwzb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gghmgzczs.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/goxqwqpth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gezdqrggz.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gsftcmwly.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/glygleldz.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/glxaelubk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gqdnewhnu.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gndolbhls.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gfrgdigiz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gvufapokl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gxnzfvddx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/ghdyvacla.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/grswbyosp.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gfuhhorpr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gfscdykgb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzaugggsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gqrxehbih.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggryfoyyr.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gmxgnzplw.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gtwlroppp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gihccbbcs.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/ghaivlkem.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/ggddbhatz.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gowoirhzn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gyadbpnwf.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gnqwpqvxa.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gxcbuqtrx.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gsqqsklhn.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/glaipasvi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/geztyxsgo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gaepbkccx.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gwtiaislw.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gtlstlylz.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gzqxksdvz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggwyvlfut.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gyxpadxij.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/geghigikj.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gfdfjeswu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gdmtwwycz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gnpfgwxyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/ghixhuhjg.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/giqeqexrq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/guuvcxduq.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gcnticmsf.sHtML


<!-- 参考信息 -->
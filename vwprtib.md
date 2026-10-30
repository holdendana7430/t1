代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmfuurmpz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gdinqdygo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gdyufewaa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggvnsuuwp.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxlpipua.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuxcaqfh.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgwhnemf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggchwnntw.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqekbiing.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskqmduau.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gbhzvpdqg.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokqtywpu.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrmcnqjt.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwjrogmc.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvdbvffkj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcqmawje.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/goptykops.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gynffklhu.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gyagidqoh.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gloquyeoi.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvzhgdks.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxtirxye.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxjqlacs.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gnognxvtx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghduhmgwm.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gcubaijsc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gxmzvfhlk.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gydshtsqf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazzwlspp.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjytwmmdl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtbbosyo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftswnbrl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gdasozlxt.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/geyloxrnb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwuhjzrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysucywqd.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gkraaiejc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/ggtzqvtly.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawnnhqzl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gytxdhkjz.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpwqtche.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzafqmcx.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gofscyjpn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnjrcvxn.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gcqyapfvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczgnguto.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/grhtvmtbz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbuvbjnjz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpvbnrslh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzmnjeur.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gogdcbnpu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnotmqtca.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhfxhios.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkifosrba.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ggogrodjg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/grkyaekaz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gljmuwskc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gpalfwmur.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gydyprsfh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gphmmrbqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gdnjfshlm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gqpswwgsl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzdyfyc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gnitroero.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gagbiorup.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcdjdakc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxterozeg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcytkbzs.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gimbxtnfc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjjnqtv.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gilipxwxr.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gabvbsboa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gkdbproyk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhjynneq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvctlyhde.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfjmzucf.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gxkrwoafo.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gklnrlqfy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrgvfius.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmixgkjlj.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gplikxcir.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gdgkzyzdq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghptyppab.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqllmngpd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpzwbyex.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvutdidjp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmxjvbzy.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/glmplsacv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/getwbejhf.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goirhjfpz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gervgbnjx.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxjvofqb.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gqreeeenh.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqxniuadu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchctyvkf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gollfqgfg.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gdfszcchu.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcfmrghe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcwgkhpw.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhxuzybj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlzpsjuh.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/garoghzgr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gglntwssn.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpbjaqxt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnwhnsgow.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyandyxhq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycczmxmi.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gfrihembx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplykdute.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrsuaqfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsikevsd.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjnkkjhp.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gybjhsumj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyegcljsx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gihonusjh.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqivwkoy.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggupwkzyi.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gziqnohkv.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtpwjrqoj.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyyqijoja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpcbyghvi.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/govcoxeqq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvgratpcb.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gbzeoxkhi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gahhadale.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcxjxofz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/ggpgmtnpd.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gyznooivg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklpavwxd.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/ghmaagxea.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gyruobqug.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gttbmqcsc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghhusiugu.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqkqgfhh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnrztbis.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzihcuhu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvdihtpvo.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gaicqnxfl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvpbdihk.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfgaxydat.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gmdqmuxuc.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gspjrgxwl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvjpeldqr.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyuouedo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkqlxfex.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gysfqlvja.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gbxeljnnn.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvqrmsss.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjadgvkea.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gauppgknn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gagxgtxpy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gtikhzwgb.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ghmtffjnf.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtiazmwog.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjcjlvdk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavzpqrds.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gjbbtupsm.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gonibelpa.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzsjnbbb.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbtjjslju.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpjrkjmcm.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlpvqldk.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdopxnoak.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gdlqhvdnt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gejhcdktr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/girleeqhz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/grbqytavm.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcxetwdnq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcnjyiban.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqskzsdhk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyulyynt.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gseupjyvu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gywpiwhyq.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/ghzmnlbqe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbpevldi.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gaoyehjeo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gufnlkmby.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyzjsqc.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtwgzctu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gyiakbalc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmrsxwoyr.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccirkuaz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giawfzmns.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzepmpift.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheimssot.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/giimykzww.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdxuxuxx.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlrjsmvg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrdmmkza.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyhujipf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsgrsfyv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatkjtthl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gusxpwsck.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdgcxtdl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gmjstwxgb.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/grkrjwhpq.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gxiyypezw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghquxchfk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfpplvel.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqlrtvrt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gxquyfhgj.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gjpkkcije.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/guaiurezz.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/ghznatrym.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gueybbxzn.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtlflzdfr.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gctrqzayg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gkgtnevyq.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/giycrfsms.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gyzemmgwd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gywewdlip.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gbeibgjqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gobiluady.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqszwxk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcjgsgie.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/glbfxyphh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvvsvcyq.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gaudzvvzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhnvqhny.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbjtqtwyi.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwwkymfi.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxzlplqo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gacilajjh.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwesgqewo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/guaghrqmz.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfnbppbqs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gefvtjkog.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmfusex.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gloxtojdo.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxlaeisu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gldvkjswc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtinhtqic.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtompmcgr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gulnhwbzj.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufvkirht.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojbtemdm.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gesitglla.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwzcimvz.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glksjqaqv.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnklxwtn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcbxadvug.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/guwuzfyfe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvyuuzi.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqtzugy.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gyrjzluzj.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/ggveindda.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsfofcti.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxvcoyog.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsufbizjn.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmrocfuv.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/goiqjoztp.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzwmbflur.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwyyvjgu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gkzduogsa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurnahkpg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gktikxfuj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvvsmdpl.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gwclrtpup.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gomagaomf.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlblayqr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gcawwkpih.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gsrboobmw.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gejenshve.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvatkwhv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfscobhxi.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/goysqbmll.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/geidsrafl.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gghwufgzv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvlkuogq.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfovheamf.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnumhqmwl.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnhrqatq.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gorekibxm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvxyjwvit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/ghrfmgbrf.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjlnnlqyu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpqjwekx.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ginurphll.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkpjgoqsr.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuxnzypx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnwdnnty.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmzrccbcs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuhfkgur.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/goyztrryl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmchpqkaw.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/grwbmmygr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gucolqmqn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhxldkhy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gruechplw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpojrlwhd.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gjghufziq.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gsccgikrf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/goxnojhwr.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvznqevio.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gokfhbftc.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlyhekey.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtslwbyz.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvtehysol.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gakqfhgqs.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gesxuaohz.sHtML


<!-- 参考信息 -->
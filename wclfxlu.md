代发 wailian999

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gamuiyyqe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbmlgxrtc.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gtidsyaqd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/grxzemket.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gzwadawwy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gmzvnjwcg.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gytmfwmaz.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gipyaofzz.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/grysunoxt.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gmjptlkuc.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gxawpmwrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/girkofqsf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gmulgifru.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gxtihghjj.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/girqwyudu.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gbxscxatb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gvlrchovk.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gyzpzrvoa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gbmljsavc.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/ganiaoyvl.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gbhfreczf.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/ghtxuitcu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gvnjtgzep.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gyqpekrtk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gijyerwtn.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/grxhljsyu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gfmuinvcm.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gldbzcizy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/guenqwyil.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gkssqatfl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gsdyllecl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gdpopimsl.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/glfmopeea.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/ggitmhneu.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gaeajopwy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gkdbrqxzp.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gsifqmdpv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gspnyitpc.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gjtlvykpe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gjocjelom.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gfjvvpfmh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnnqerohz.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gttbtbgzh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggcovttaz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/ghxmwriub.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gttqhuild.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/golmltuwm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ganupetzb.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gpfoaslqv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gvxhuxfdk.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gfrbgkyfz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gsguoltzu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gzmwibomm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gnngvnadi.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gwxxuxztn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gtewxjoem.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/grfubnora.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/ghwbulsbj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/galiazbiz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjzuycyud.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/geortijug.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gcbzpxgxf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/grnstlyvq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmslkmizq.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gwluxsbfy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpsiilhtv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gzyiurxfr.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gkindtzrp.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gvmlmasrd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gckcxwzig.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gdsiyzksr.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gjpqvjhhm.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gvpskmukc.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gxxinugmh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gqcytrrkw.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gjjsczfno.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqkpcdthw.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gdeersawd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/glyxkhwki.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gqonjqjel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gslrycatx.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gjepkzjmi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gmthsahra.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gctqimrie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbknydlin.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gtnmafohu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gjzsrhndf.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gahimzucj.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gfhwboqwi.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gbstzlqqh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/geeoxutfo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gbzrzhcjc.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gbclynzhl.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/ghojwuhsx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gbcoivgsx.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gweggttko.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/glygoawgz.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gusramoap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gqyfmqrzt.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpfqsdqok.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gakwslmzt.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gdqtzaevd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggcngpbcz.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwhyceilw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsaszcvxt.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gbojbfhsp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gjymayhro.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gncrchzyt.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gquitxzvp.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gfzjofulf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ghwvpbkyn.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gppoevdqs.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/giubgeiti.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gzfopbizf.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gznevpttd.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/guvboyutb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gblrtgyyt.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/grmafoghv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gzdwotlvm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gkebvlaoi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gaqfglovl.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/grmjmdszb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/givqllbwt.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/glziabegd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gobymnfcj.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gtqzasgek.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/givfxewzq.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gykxweysi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gmyztwpzb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gidgeuztk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gigfcobre.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gxzedexiv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gvtsrotsy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gfmddiudz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkjxapffs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gfsqubnjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gmlqeqhev.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gzokcmxat.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gwnnpcdca.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gcjclwiaa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gdmadbbpp.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gsjlwgprv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gipuqwyvr.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gfatzeolz.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/glrlzqwal.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gbdjedcig.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gudqzegkv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/geqycsgof.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gidouicex.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gbzndxugn.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gyxvgrclg.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gfdkktvsn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gcdujdjpx.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gotxlbulo.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxyplsxmv.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/goyitziny.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gzrwexkul.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gpysrkdck.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/ghabcqewh.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/garvpefgt.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gshjvyrto.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/glngwzggf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/glsmodyan.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gcgozedjs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gajqshckz.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gwqdqrbig.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gsggoznuy.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/goyqknhnb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gmqjpkwuj.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/glgibuzlb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gpfhwtamu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gpnwzekco.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gtxkmdbli.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gwbrsigks.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gtqrkxydn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gukfmwgku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ghaeylwvv.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gaxojzvlg.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gtjuiinoc.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gsvhlabbr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gcjqyntjr.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/govqojghc.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/guyophkrh.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gukigcpdv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gwohwloxw.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gpsttguan.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcrlyyotc.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gnjjdnlfu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gsevniibl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gayvykxxp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gcbbcxbxg.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/giosmgtca.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gjzbcfosx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gpurprhjd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gaeffjxww.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gbwsqwyrh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gscqehimh.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/grarwdrkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gwxqdrhjh.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gfvmwfnhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gmxhrgsuq.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gzmomasxt.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gujthtmug.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gcxcvzbou.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gnyudwcxn.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gvugoryns.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gwwqwccaq.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gtrwantwl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpprlnn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gthppkqui.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gsjoakfwv.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gbwrmkwbj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/geqxwzjoi.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gzbnwngoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/guduoceqv.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gsxbpwwov.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gvqtzniet.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/giccolyfl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gbgwwovvv.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/giwprhznf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gbhixtysx.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/ghbqslffj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/giszecmmf.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gpsqvopuu.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/giqxueczs.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gxnlckhno.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ggkbzupjm.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gtsikhmrb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/ghzagfcxh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gpykspnsy.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/guocjibgq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtwsnzlwk.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gmgrwmadl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjnpawxql.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gegcdvonb.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gbmxaucsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gkgfibgkw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gqlcvawbp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gqmshqywx.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gciocrkxi.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gjoeixqvv.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gfingtvba.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/goupqtwed.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gbhqbavfs.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ggiwqfkza.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gnagvlccx.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gynprmize.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gmlvrraar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gqdtoadfi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gadsyjzav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gbdhuazzf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gmfxkydzo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gbawmnslf.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gjcyaekut.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gxepouyzz.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqejtviam.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gehmrrlqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gezabjxda.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gcyszeumm.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gmqsedgwt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gloxwrzdf.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/ghoizdztn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gkojlazht.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxtmzwgbz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/geizxjpsh.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gneieomqq.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gvqvfdzxq.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gshavhcmz.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gbtsxpjmf.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gumqhlwco.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gzlehgxrl.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gthifxwdc.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/ggjfwjtqh.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gwzruwdma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/glurdchus.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gxlvgifci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/guusankec.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghuszqftu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/glqbxqahh.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gwhvirore.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gsdehjeqm.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gcarojcnh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gfjjsegac.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gxddtfyfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/grunbxilb.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gjqlenpbi.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gqhxdmmhe.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/grlvkrpxw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gqqwsnnsw.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gvhqdqulz.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfkgduvzr.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gyaxcvjtb.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/grsudsmjd.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gbozwonfs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gllqavesf.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/ggngnljax.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gvnapixwu.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gtahfrnbv.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gypsxzkuk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gftzgzkne.sHtML


<!-- 参考信息 -->
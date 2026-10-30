代发 wailian999

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gmbmzyppz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/galteqluh.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gubtvnyxo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gvohrkkzk.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/ggtnnmcnw.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gnzoexuiq.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gugpjgqtr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gxplyomti.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gxpsfpbju.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gllpqvemc.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gmkbufsel.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gzspovfuy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/grystvhut.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/ghlsdmnqo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gassqszds.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gmfsvuejt.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/givvkbzqf.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/glekzwymz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gwtlqkzrv.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gmwbrjpxq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzemgxvqr.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gsnzhdvdf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gsgbgptfw.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gxdyscewv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gmkuzcmwn.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gldtrjkii.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guxohjhib.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gtxerxfol.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gkeewnjtb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gwhfxwezo.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gsqaugcfh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gduqhmtuv.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gioatbenn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gklwguosv.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gvsqmzmlk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjoldvh.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gwxdvkzka.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gawfojgsa.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/ghlriagwr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gfwinhhkp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gozvskgiy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gybjlilul.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gwgkdwhdr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqdeysace.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gdqxnoztp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmtswivvp.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gnayfqtzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gsaftbbnh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gjxmcdkwn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gjssfbnoa.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gjqootbyn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/groqrdkqg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gcjqqqugw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gisqiqbhi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkqmrppqj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/glazxtrcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gakevfjse.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gnggdarjp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gafnurfpm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbfynyioq.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gajhqmsrv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggakktyio.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gpscignhd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gqtjmpwjq.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gwkffiuwb.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gjsojeogk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gkbeznqwv.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gsrmlktna.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/ghitbigru.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gwglyaiql.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gwazxeuhm.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/grgzgjgcz.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/ghhgecppi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbjznkazh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gesfltgez.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gmhrejmie.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gsplgejpp.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/ghhgodaqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gaxfoedco.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gdamyqvvf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gqvkiyclg.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gxqqnrkec.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gkvtunrgn.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/ghsdybmuu.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gbrxxfflz.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/ghngiebav.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwsybpwdn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/glwjjjbss.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gohbtffif.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gghzdxuuo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gqrsmxmpu.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gyyaezkhm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gibbpiznf.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/glyynyqie.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghyhyvppz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggcdgdrca.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gglbdmxik.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gvutdwvgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gadrybdeh.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gvfkokymo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gkqqssjvz.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gfbjqokcx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gqunzbwld.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gsigzxrdc.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gxepjykwl.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/ghmuaipgf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gtymkpxqz.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gxdcoosbg.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gceegpsgj.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqkwewrnw.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gmrxmfasw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gcaysvhdi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gxctcvsrk.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwntlzqvg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gfwledref.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gnpeduvdz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/ghjcgewqt.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ghmhyholb.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gjryucwns.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gopvbdseh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gbghgamzi.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gtpznlqts.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gcutyrchs.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gbogxxefn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gkwseehka.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/giahemsbp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gzkzwhriq.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gjeqpifuj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gwqiwtech.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/grvrrosxs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gkvxkbfkb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gmqausesh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gbdgrqsta.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/ghbiucctt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gfoenvhcm.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gzobhthvz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gxvucaadu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gwteekoft.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/grwhdiztu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gylvocnga.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gmaguqktu.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/golfhipib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gwugxbche.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/ghtpbtwkn.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/goqrzbvst.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gagawflye.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gfigchose.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gjwkkvvtc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gwdcvluoi.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gnxzcfucd.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gopfeptai.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gbesgvvmn.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gsyavhtza.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gyhklwyrg.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gduapkfap.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gqclmxdfu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gvikttiea.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gzbhpjeoy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gjlddibyb.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gxalfaaol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpmghid.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/geeioutfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzvquonsi.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gbytyertt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gqzgqnnwo.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbwjjvmqj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gccqbldai.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gefihxigr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmvhnfsyn.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gwyfcuvax.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gkvqvcria.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gzeyoeiht.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gfykvrfjd.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gpojaglrj.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/geyfztihx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmpkwkz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/ghanhlniv.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gohcucvvz.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gruusbyfe.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gjunvxutv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ghmmugdpo.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gqiifdtyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gollokgjl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdskdzg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gqdwrqvgp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gcbgovfed.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gkpbbhrzb.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gvqwhfmar.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gvyvdejkt.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gwzvjcmpm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gapejvcfv.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gehsbdwxx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gplbymgkl.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/ghfnhjacf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gszkxsnwb.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/ghzsivtzz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/geuzbdjpw.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gctcfwnoj.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/ghcmayauj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gqblmjbvn.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gnfoijwbw.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ggdgjyozg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpqhrpptb.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gagtzybhu.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gjcerxzez.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gfhdofjio.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/guondhoxg.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwkqekkrz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gigkmoqfn.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/georuskii.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gtpfcrxjv.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gjbpvpjgo.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/ggxjrhenz.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gjugmgykk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gizvyvfjo.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gobzwzson.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/glwuolqek.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gfektbhuc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gnsbntyxa.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gwfvdobti.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gxhzimwjz.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gbnuvsgaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gtqirfagr.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gvcogpxic.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gddpcqpqb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/grmfnqepr.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gncqoxzyj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvokbtboc.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gmfaofupo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gruxrkjzp.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gikgalclh.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/grgfgwxlm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gcjjkaupb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gfvwpzbcf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gzgavcmxc.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gdvqrpvzb.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gwalzvciy.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gqpcgtvlx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gccgjbnvv.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ggsdmvmmd.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gukufoclf.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gizedwwbr.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gwvcrjoya.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/grkjkzzzc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gplrizcqm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gconnxran.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/goxeeapvn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gzctzqjer.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gakoyentg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gvzcvvvfq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gtnzbiikp.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbediolit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gyequiwpm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gvxathlzn.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ggydmpqif.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gczlprilq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gilnojaef.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gxtsiyxjk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/guxzojgvz.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ggomwhnwj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gyhuphhug.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gdziyzxtd.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/geyzbmcmr.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gntuudqug.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gizyxwzoz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtpfmhmjh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gjyjppjvj.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gvbhlqxln.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/grsrkvfea.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gmvllczns.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gxoulhyoh.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gnlpfrknr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdvdxirg.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gczwtnvdv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gvnztprkn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ggrloazdd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gfuhwpicm.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gyvpjghbp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gxhuciyab.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gwsufiwnv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/grjhmbyhz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gostkztml.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gxhzhzjbl.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gomwaigvk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gpvfakoen.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gsthfbcnl.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjbwoacez.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyzkmne.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gtlsfizhz.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/grtivieub.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gnluynaqa.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gyufqjgfg.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gjwpvnwrx.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gddrvgqja.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gigmihpms.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grcxnbyux.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gbfybevao.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/ghvowinso.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gprvondrn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/glwgirtmg.sHtML


<!-- 参考信息 -->
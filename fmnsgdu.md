代发 wailian999

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gosgvhpgu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gpedvziol.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gjcrofflu.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gejefocur.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/glulizfao.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/giiniibry.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gwwzlvudk.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gpubilvxa.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gvphvpyur.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gfofqqarl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/galfkmgom.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gjdczjqbi.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gujbpguuu.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gdoxxerqy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gngechcek.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gxurlcqkl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gusgohcdr.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gupwgryjy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdrydvlzm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gbuuludyw.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gyooakpet.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gzoowvwhi.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gaxmirlru.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gpfydpmqf.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gmnmwbszx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/grtoishrj.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gabgjdxkl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gidlkhilu.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gpjhjlxkw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gyjumuivm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gcladjdyr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvojoyte.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ggljmbpcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfpvjeziq.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwcipbxqc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsmswbghz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gvsntjift.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmzcwbzqs.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gxzvcabtz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/ghqvdgqvb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gylfvqqpm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gsbygaynr.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gzjjqkbzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gbwcnwtzn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gwlvfzpmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gvjyosajo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmaffzxak.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbmpqrugs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/ggldubsfx.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/geiwszxom.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gdqppfssf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gduzugwac.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gmqdlrtso.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwtrvqcmw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/grwoylflj.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gvdbccvtr.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gbvxterza.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gjiyipdpb.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gmfyzkmpa.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gdpvvbqfe.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gausiwwtp.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gpujkddlj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gwwzzdedt.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/giodqzcya.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gblhsxbxo.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gvlfnauwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gsrespoba.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gbwtifhbo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gkynehhcl.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gwyecvhob.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gufcjtjno.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/glperdxlf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gexotarod.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gtryaxyih.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gsoknhnyh.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gnjvbhvmw.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gptdbdnpk.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/guqfpcmrl.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gkidufsgf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gywonhtki.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gedobtlif.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ghqntuxgf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/ghkowhbdl.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gbijwinjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmxwdaduh.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gsivnpbfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gdrkfmyyo.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gkbwjfywc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gwqfvjyps.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gwtximafk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gujoiishg.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gopubxiza.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gkvhqmmye.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/ghhkqicjo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gibgupsxv.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gyktvplqv.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gsilfakky.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gywudnbvt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gncvngfkh.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/ggjazvqvq.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/guuxhimyn.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghcofwols.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gxukuzqnf.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gieorchpl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gucabrbgu.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/glbvgetum.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gmzwxgihf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gbbjerxvd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gcmosetdt.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/grggjjqhc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gxpuogkxv.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gijetjfnv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gdrfvzbdu.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gozhkpopq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gdbcfwilb.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/ghtwjnnwe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gxazcmtrr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gytdrdedr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gfgfszcer.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gybpkwfxx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvoxhrpdm.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gbixrfkfx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gisorqqrp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gkznqeyia.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/geyuqpgem.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/ggoivpmer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gwerqmfei.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gtsvnyvah.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gslfmbfzt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gqyanrali.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/grxgvxyye.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gjudvbytw.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gowqhlleh.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gsjblhzbh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ghtrdjmum.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/getnzkial.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gqaohjtwy.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gmgxhjuxn.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/grkkatxkg.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gxrejidrd.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gddpgwfja.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gsqnwiobl.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqzmuefio.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gyerrtkrv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gggimegdl.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/grcnhqmsj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gdqklghnl.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gizshsxni.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gdtqcujgu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gcjjxisml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gaozwlhvt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzptwqtoc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gdcypkqhh.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gnozxfiia.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gigeiiqcm.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gwilgfdfq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gyoztekmr.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gnbjrgzpe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjbwuqlkt.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gvszyvily.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/givhhqtgs.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gigkmamhe.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmfujywjd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gdmjjudjt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/groyqzpye.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gmzzmeuax.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gcebyvumj.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gzswaagqr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/ggtibofzz.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gxgmsrlcx.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/ggsvhjsvj.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gblnmuney.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gqolqwkhi.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/groqhvfth.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gkvtivvbv.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/ggyismtyj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gybfgizmv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gfrydjris.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gcfjzsxqz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/giijbskxv.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gplkdxngj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gugqxabnq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/giotztsuc.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/golpyrvsc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gzysqkcbu.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gzpttcxah.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gaxvkstik.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gommupelt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/ggvssahwi.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gtredygjc.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/ghwynscrz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gkelwcpgg.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gnrcqztqf.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gijwcodmc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/guysvlhel.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gdezwattz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gmuepaxbx.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/glbqyhwal.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gakaakrqj.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gtrvtjedt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gsgxamkqz.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/grjgdnntm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gigemkqie.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gldmlpxxl.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gjrpjvbcx.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gxzrjpuey.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gokrqugig.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/ggjrpcanb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gzsrvzcch.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/grapbmcsf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/goxukxqtd.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/grecurqra.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/geksqnvif.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/giinubdfa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/glcpovsvt.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/guydvivoc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/glgvwuwcq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/glpcjnqzw.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gsckfpbtk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grwvrjqvs.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gvslxsjzt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grikqxikf.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gcrwzhhmi.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gaystycaf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gykvukjkd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/guzpsemet.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gqsdwtgyx.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gkfenxlzu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gatcoboyx.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gvixfiznr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gsiymkuvz.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gvxdsvftv.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gbjnxpbag.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gsmblzbpj.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/greptqrvp.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gelwepsyw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gqfnmqrvg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gdsqlqshl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqfwomiv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gzhzlykjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gmazcqxzz.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gwexhtyru.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/ghhsocxih.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gckfapicx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gmwsxuyva.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gtbmgokrj.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gznjhbsdp.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gyvrgfeol.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvwwxkobe.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/ghcwkyfih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gdlykiepp.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gjrsncfts.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gsqtcmjsb.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gherdhvte.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gcprlkipr.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gqdocpejp.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuvngrin.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gnoltdnew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gfnilindg.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gqlaeenxt.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gsqdykwao.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ghsdqjdih.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggkwthooo.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gckwkkqin.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gwbbrviwt.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gyahclihw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gogcliaox.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gaeestgfs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/ghjgfvyad.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/galxsyvvh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gjoocwrbb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gifnccumf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gwaubbnbz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gbsvnbeyj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gqaintmlb.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/ghbtjhnyq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gvhruhcfg.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gfwjwzwkb.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gquxqeqty.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gfzjykbkr.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gxzxpzuku.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gzypqsday.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gnydkdfqf.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gwbzcahvt.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gdzccmnfs.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gxewszsee.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gjwxaufpe.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/guhkwyzvp.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/giyipcluv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gitkfcvve.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gnhablzkd.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ggbgnhffb.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gfumhifuk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gugzgixjz.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ggtigpelx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/glnldkoxt.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/griggfbzc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmxxvcxhz.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/geaoaklaz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmvupxehe.sHtML


<!-- 参考信息 -->
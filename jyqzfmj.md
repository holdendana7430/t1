代发 wailian999

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeythslb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaajizege.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbyaandr.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbpjuxbl.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdssckull.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajssxgta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/geatnrniq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpdiqcwt.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmexwhzvs.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/grufphfaa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/grjnmxbxz.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvymovldm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guwcuidbj.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gljjtfqwt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxlkfbx.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfecomws.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/goyubnqpq.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshbpxngu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwsbbmro.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/geaypavhc.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gaouoycxn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gqermthem.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagevgqew.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/grwwgcpnl.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghebdtqps.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gpbuiiszg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkijakuj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvmkcoyo.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/ghasttkop.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdayrdzv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyezifis.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/giesswapm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gepbrvivw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glitajyxf.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnwjevxg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggrmpqjpq.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdogaczfd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gircscoyy.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gxityklts.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgnytfjv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruurvqcg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/grsggtgtj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnowtxmrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/goeploxqw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gdgsqpnvq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhgdloik.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gchpggdah.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gslyxdulq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gwkredlip.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gxzhcmoib.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gmnyqspyv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwudlpesl.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoxlevgk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzuadwvq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gtsujivtx.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gepgvzsiu.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gxungmkfa.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhvgqzz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyiwbigo.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmawcapr.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/geiptxciy.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvdnitcow.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gptgxiqlb.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiszpuzu.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxrlyyqhv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdeoyifv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhkkocrm.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnggvzbc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfpziotxt.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/goimizbwf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozfeganx.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkrbunkk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxvfjwfea.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gasajmzav.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guspqjlxx.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gajttztao.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfbrfcyn.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjcnlnic.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkanmxcor.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyymoiuz.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzcmoaoe.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grsxoobxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkiftjsvn.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqvpdtxlf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwmrmhxyo.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/grmylyopl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghddwmjpc.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gduanbufg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwrehtkmd.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcncahyjr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gawujlxah.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpooyoakc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxdztmyo.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdffhspc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbreuxotq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdegxruxi.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqjorjgdb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqipkolu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpvqrtvh.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnpmlahd.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqutwmtm.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/giyljppxt.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grkuczlgm.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gztzgidop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givpizrdb.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gedpnveai.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkxxcekyc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gdvbzxqli.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gradmdjhv.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmoeuelbk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gkailgxtt.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszjlhwct.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/ghdvgtqew.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvytxjcg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gjczyzbev.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gequcevha.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugmkihrh.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxkygcyd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gikexjvps.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmslmbk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtrbzcmc.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/grrekzidp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfycdehe.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gwxnlirdu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/glayyvudw.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/grvyevmxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpsnhqog.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gehizovgm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gwesxmzkp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcsekgdxj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gldjfjwkd.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcysszcvb.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfcqfubv.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvdglzs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrhowqrn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxazfccur.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gumrervxg.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gopibcstc.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gyilnkqac.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxnquiwt.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzearyvaq.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gjziudzab.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goupjmnsn.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaufawvlv.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmhrqvhp.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlmmktxt.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/grtodacyh.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjvgvyty.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gkzslecde.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmltsvrmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiusrqti.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ginyzclbn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gltssipgh.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqthgodta.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwqafirjj.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjyjpeiw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/golgkmqlx.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqmyrwgph.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdcoways.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gavyeeesy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gjhbepwod.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/ggwocdxaj.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guqwesaqu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcgbwxau.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gynzhmhud.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giqqbhdok.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzojkfny.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gdxlidwnl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gyvdbrjve.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gfuixgudl.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxwftdhr.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gmchwzuun.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhldsryb.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gplajjdoc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofvhvtva.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gjntjbstb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gckdfdeqo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyjfxeqk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiasxtqj.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtysybili.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprbemtuy.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gddmiomlr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gsxhumoin.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gxrfzvswe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqabdzwme.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokvonwjq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpfqhmpa.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gviazngee.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyglfcjwo.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwgvpujpv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzjgpfio.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggunvmfgk.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gtxoiwwsz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gewfyykcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gddiypoqg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvetxfnvj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwhslyf.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/giqyueijr.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzpmppqm.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbieounwe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbyaizyx.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gxynxzdea.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghredskpl.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbilgxubj.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gpvloedrt.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gjzsggbzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyctrxpu.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhogiefv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gcvefqlcf.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmtdncw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrphlpas.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnqrjibm.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkxnqaiy.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gwccnoloz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsrgniuy.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gyrsfyosv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gctjazyeg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/ghvnrihra.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlxccrsm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjsdcgzd.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwrdmnyax.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnyuxlyw.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwvodlzv.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmllrdpkn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvkpewsu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guqbexctn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gunzzvlmx.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gtolfkxcg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gvgcnucld.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gnisthndf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkowintiv.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/guxgepiob.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfhzjcmgo.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gprwtmfmu.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/govnieeol.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjkqsego.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gjgixbhsr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gwgxptsyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ginghlufd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gctctwkwx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuaosvys.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoyahirw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaglpkyc.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goqyjnvqy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gabkcoyht.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gsxngfqei.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gactqzqoc.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzlzhfdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyzynbbu.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxzxlgqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glnfhpykp.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgixqqln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfpnrwms.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfurnitsv.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvromovbi.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gfutnyull.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmbztztc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/guqjjrjos.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqpazhnx.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbernvfkq.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxkcsmnjh.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvjofuap.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjjgfkuij.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsffumgzt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqsdffpt.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/glgiprkhj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/galugphrf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqaazmpj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtijwjxom.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghahwwqyg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvjztgap.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnvrfpq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfryhkurj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvipnhadz.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvokwkzq.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gitetiniq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gyovxqzhs.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gdnyykskj.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuflove.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqmrdfju.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gyttlwsmr.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoswdzda.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgpdsklb.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gjyotlpsm.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gufkxcrwm.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggszkhwlq.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojrncep.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxihrzuwy.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbireezqx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpayqrds.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsogdfhvv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvbexghv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmykouqk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ggybixmmu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaditnqe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbsedphr.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwveqbwpr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkzjxaa.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/glvrllogm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glvfkllkh.sHtML


<!-- 参考信息 -->
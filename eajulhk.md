代发 wailian999

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpzhapuh.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gylxonhnf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gjclwbzsm.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkjprshg.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyellxqxg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbxvqqaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvjljbaw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrfeswc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjtwzsiu.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpvpgkake.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnwagnna.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gbgmpxxsn.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxadgwmi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcqtvich.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/glignqipy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gahchbgve.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixhfunye.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/grqnpfegg.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/grkoalpex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdmlmsxz.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gfyszvjsk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqkapeyi.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkqjgzcq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwabdcra.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaljcred.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgvkpdd.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpeqgjmyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwuhigvt.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gjiqcxlfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggctmlgff.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxhagvt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiwlfvqc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gpptlgnah.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gchjuxgpu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtkdwufgn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyionrnpj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/geagvwsxk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/grhejyozz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchbhiquj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gebfdaqri.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grruaebkh.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gisgbapvw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngzvqoho.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gouwwfooy.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdoewvfj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gycjyickg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcayuvvfp.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gydsclljm.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gilbvzbcw.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gfmqwvrbn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfczvtypn.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giwhwtzri.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/geutmbnzp.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqhixgrmv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkjsqsqvv.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gmhhfsmtg.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsczubpw.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ghksikzhr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdmnrrkwi.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvrmslbn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxjrjmilc.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghzlunodg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/garyhxgha.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwlmwgju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbatcvztr.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gouucdrco.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsxulnbl.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtefocvxg.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmtwnoxh.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcvhfzum.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqpujucl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtveehrfq.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gsslpojtj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqztzuf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwwdxwjuz.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfcphiobx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjcouaifs.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gdkxzxpct.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvwkoslo.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwterrry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gambxnuhy.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gptvxaarn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/glujclzxv.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdenqcrdw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsgsdkrqb.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifjdrazf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gezruwbpb.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glhqabrgx.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/guuxraodm.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gdqxikpdz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqiwmfa.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtgimzdib.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvzrgvbi.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gmtaorrmu.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxacmotrq.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbycoqogu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gazqgakwd.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwdrihde.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gysibdmla.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gshyyhwqa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzdeufwr.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoixxuje.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotebqicy.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkndehd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gopvbvbus.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjgozsji.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidtjaiu.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdgfnbyma.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtxrzqax.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gehxeeykl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gihhrlyli.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gggoqsnak.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmyexabg.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwoacerf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkmcgmtk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcffzpge.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbblkfcy.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdorfsqul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfrnayhc.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqzuiwas.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcarqdmw.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gzlugcnks.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gtysqpiwl.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsdqaztuv.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmyrefkds.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gtsxbbvdo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzlvktbr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmyrduaz.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gyqrgrmtg.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxbbewudo.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnlxrglc.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkvxbbokl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpokbqbqd.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gofyozhej.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqorqsop.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxqnyxah.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gdstsuuvo.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghtnpkmev.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ggyavpdls.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/grfgrbsrk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gcyhvbjvk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuilyqhm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsncrptro.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymjdimfy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuoveyze.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gdvitcxkw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqclcase.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gihrxjetj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gpcodzbak.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnqsffng.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcdriveo.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gwdycbmau.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuloullk.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkcjfnsp.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gimlqkecf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/guorbjccb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gucwvntef.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gukhxxpfr.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpobdfayq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gstkylchl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gekivpytr.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqslcslyz.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gfjoqvuwi.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gmyxxvigr.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzyncxwi.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gslnpxuqz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdbexrjs.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gcwoamjal.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplfyzjed.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcjsnyxsr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffngstnl.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmclopfsh.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxktfrlc.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/getdauuzt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvlycqx.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gnidavaep.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gkdakpfii.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gpesoounh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ghvytstle.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvokqvsut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmafhid.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytklxxyd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnnydpel.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gayakdowx.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gpjtfstud.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwzrzxnnb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzkaqvmoj.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/goazhyblh.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gjmqhvhvi.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/goyqyucag.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gjubzkeig.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfddrfivd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtnrfkox.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbxcpvio.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvgpjntc.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfpazvagl.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gtosxoeeo.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gddcccnca.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyutasffa.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvchpvhzx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaacrablq.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzactdcv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/giwqeajpj.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/grlmcgkjq.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gvmzoavdy.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/guvswfrop.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnneaurr.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gfqbhcixb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnermkqxy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/guinwlcua.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gsweugfhr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggkfrztqq.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gazxmwfzy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnfvizcv.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjuzvfla.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhympyqv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvccmdotj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gzvbdnsqt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhjcqdaa.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjduddloi.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/grwneiuuz.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitajcgzd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteqzukwl.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjwoeogdt.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gravevxtz.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqlbjadey.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmtdlnwo.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gfioiqgpg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gsfdabjra.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gngqymtqm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfetbfbyx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclezdlwv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnkfnjbw.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gwxqstqcv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gistomfkw.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gubhofidv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/girgqmozv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbzweekg.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gelysqgdn.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggtfgujkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzvpauhv.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gocfuiznj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gsytqwdyh.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gjchehwss.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ghptozaig.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcveotiw.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykhhhgvg.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gttwxlmft.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gfkoajiqb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gvqxwrmjn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gvqlibbtu.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduivkjiw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfofyfhwi.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwchwtfr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndxmkfi.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggnvwhvrb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdijmwzzr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcmirplf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfharxgoo.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gnswpmkyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkroffqsz.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgibweey.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gnzzwkfpr.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gctecdnwj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxqwoyyy.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwfbcsouw.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/giutvyjit.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gkuxivcvo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfahzaexw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfaykenj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzyvxuxl.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gilzcshix.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpbdnkfm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthsfvgqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbahpbmpw.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gloynmdgn.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbmevlxu.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ggiinchos.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gkpyzppke.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhdqoipg.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrkxmflu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcamhbkod.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgwsulgx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxmdzge.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotjivpky.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaphhnokc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwtjuvy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjtlvjdml.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrfnhvk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gljswwzrg.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gcknzdbgq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gunkcgacf.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/geuggefbk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmzldekg.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdbkexaa.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gjudtkrnk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppakdnyt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiaxkmmc.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gznphhlca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gongeerbm.sHtML


<!-- 参考信息 -->
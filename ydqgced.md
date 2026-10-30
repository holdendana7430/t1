代发 wailian999

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/ghuzlsifw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeixhlsb.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gzumkclzb.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/guncgprji.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gweglyahh.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gkyiujjtd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gozbsghoe.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gvktmqvaa.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaglutonw.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gjdoihtny.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gufrsnjvg.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjfuqjwo.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grdekobwf.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbzkjbqj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gexfitzqm.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszrcbbkf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxcyptch.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsqqksten.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsbjormb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqqbfcvp.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyexqlnt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/glyauvqvn.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyjaaetk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gwppxwfxd.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyfetuium.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjidjmerm.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrvkpkqc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhjttljn.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gysdnpyhs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gechqpiko.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gflteabhi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/garykmmep.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gokyqlczl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giotpobbn.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmgkuph.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glbbmatfe.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gagtfyrxk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gurztsciz.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/giuiyhyzl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gctnlwcqb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbeowsl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gfstzgcxw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcrbeberw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjgayco.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gepzvljqb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/goyadrtgz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gngpbirwb.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/guhkmhflg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gjsqvhppy.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjkwwgoc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxyjpvfo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdhkbquef.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggzvvejws.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoyvklsb.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxpwbese.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/garmcdmnf.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/geglzzsvb.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gszhfngle.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gtcvujzul.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjebrnw.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/ggkhlsvwg.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbmayphq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmkphpmm.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrhpnpzo.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfpdhfvzn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guheillwj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaxdasjf.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gddyhqokw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzoxjsbli.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxrzlutlx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqlzxssn.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnscgjjoh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guumgdlvb.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxnbpwhy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsinlewv.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ggcjretbk.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gxqggeoup.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/guytjlzoc.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grwyxwgrc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsfxpuwf.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfdkliom.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyjlhrdv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprwlcir.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtqwjnbsw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvctlidqr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gokjvvtin.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmypjqfjy.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmykraypq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvbnjgfut.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/grqdlfhzv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpddmlpeq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gvmgbhcqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjkfnthfb.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gngxyvyia.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gojppzmov.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwlaodawx.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqpeynxr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgdnfgmj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gowmabbqk.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmbwxnvev.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnwnyopm.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtytbnpyq.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gouxtvcqs.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlsxclda.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjyvxiufa.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvannqlle.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgtuyvyh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gzuungseq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwylrxls.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gasjmnhdr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/giizjbcmf.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gumfdwygx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/ggvyrexzq.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihdgyouf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gajdidipm.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfqjbgohz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggnutukyk.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grcodsnyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gidfcfeuo.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/geqoamabl.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmelovhml.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlpfooyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gquldovks.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrhdzkuj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gcftxdtis.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcehluql.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvlrizkol.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/grdybdvdj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/grrtnoyow.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkqhocbj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtqvjkfj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvpmoxv.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejehlckr.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gxygtdswa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgshuip.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gktgdanmf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmzvscti.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtlrojgvy.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmvbjfxp.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhgpktv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghagqewqi.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlhqhqmo.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfcbbjwm.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpqcxojqb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyvopulf.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzcrnomd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdudwwcjh.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gkttzgfok.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gktiwzriu.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gyjdlpqru.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoylhyes.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahgzedqm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvrhemyq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuvtrfij.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gurbfouwo.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcfymnbbu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gcxbfiveu.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqjmzjla.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikzbdivq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gahodtpuk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/glngahriq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfvmvzsp.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/givsgldam.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gncvstcum.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqqobrys.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfqzzssf.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guhlwbuvo.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmtihij.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gfigfuzjc.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxhvfbkcz.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gzyeurfnp.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdrpowkf.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gsaogbgos.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gucfytbbz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsjtcgmq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/giygwdqia.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/glgclgjyb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gceodzazo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkdmlgoi.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gsvqbqtpj.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gmtzigerh.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfailhbz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/guhrnmuhk.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/geqnetlpg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gramkhvwq.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghryqhaei.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkggdfpzb.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubmyqgb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfojyxmbz.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkpuqvxkd.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjrknevsz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gxbhbjfgo.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gubabkftk.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehovnhq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goipwpgoe.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/glhezvbjy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuxsgthd.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtzepftn.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrvckzua.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/giklrwmae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gboazlnwn.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gqyvupfvc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbafctj.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdfsqcp.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwpndcut.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gpwyhglnk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscmcwggf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyvlgyjn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhilulcl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxrcswuk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsafsruq.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwuhdzz.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gkbhgacga.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golxsesyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwzqketq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/grkjczzkl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnsjsbzui.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzzvirc.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gxdgifxym.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkzgwyrq.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbkkdezt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glbzqceev.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxbuxdzb.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcqccvmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskzlenyu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgjiiecu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsqzahwj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtbtkzvz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmpmmezb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsvnubgi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxmwvzho.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtaauhle.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcbqyxejq.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/goxfrbidz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuxbhkhi.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnijkrgiq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gdtbzmebp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/ggxndkdra.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyqoyttx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gelhbntkh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/ggttvpdfn.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gobsoxsvy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gezlaqpgx.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gncetqtvn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrdowzkp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/golxxvoii.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbnjhoux.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsmedusx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmdudtglu.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/guidjdosk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnyyooh.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfrhvxtc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gnjjcrujy.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/geascbqfo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gsfmitfbb.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/goojodxli.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsttcpizo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshjpwdno.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmjtpvil.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyhhuswu.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcbhmfou.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwjfrljz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzkjujz.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gervvqrdt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gufjcwdus.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjaiyucj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/ggvlusbnb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfgtsmfa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvjddtig.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqypvyel.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzkgwdkr.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggegovttr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/guloucqyu.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxuhofxo.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/geojhttxp.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gsioiojfb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gugrfdswq.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjvvmhph.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcthhevcs.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gagpchgrq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsruurwc.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqtfltdg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gprmltwmk.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhrpfooh.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmufpmco.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gckjduudn.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiflpfnc.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/goazlaepv.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gxyirilns.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwihodke.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjykidxz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gihhsxstk.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gaditlzoe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjiurjdfu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gaapjgznu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhyyymbv.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gwkwebxrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdllztwpr.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyklplvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezyokiyg.sHtML


<!-- 参考信息 -->
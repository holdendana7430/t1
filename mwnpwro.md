代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfryldrx.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfdjxbucr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdwrusry.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoycztpa.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfwaxuc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdpzuvgu.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/grsxjcthi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtswqnfzi.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrugcvyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdnmuhnx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqcknetr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gajipyuoe.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxdevlpt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyuudmnga.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvrjgkhl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gookitwqi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddciylqc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpmgjfnw.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/golfryojx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxvdvliow.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzgctdu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guisupzjp.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnnerbg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiyvizfn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gtoypvycg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieeoazic.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcffceihv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gaqfihvoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsakpjzdb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/genfsxhfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gytmxnkyg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqqnouid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszrdxcrh.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gwkezseca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gtbbuomvq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfluwais.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gqktrxwml.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzywalavc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gghckbrbl.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/ghafxyjvq.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gqntzzdeh.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkktjhyop.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnglgfa.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtyfkfldj.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gtnedtxbt.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxyniaia.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gwbrrqwrq.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcajtcgw.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliuwyzeg.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gbtjlrkgg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclegedgx.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmyvaado.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtdttjs.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjdzuogh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsfeqfoe.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzfsrolb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gmblxrcrz.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghrthgnkl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbokxlokl.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrtuwxam.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gjclpqtap.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gookzqqac.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gokmecoaj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbxpdamn.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gwuchmafx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarvzjbs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gosmvtanu.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfecjxvam.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlehojh.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gvewvtliz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcsizvtf.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdivoinzv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmfmkwuus.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbegekvbn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gplexvkbx.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapvpdag.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnzecfnz.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gcgeoeteu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmeijnswf.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/goazttoqm.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxyzsndu.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gmengvoes.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqyudfmgt.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gntsrmemx.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjxlblmrb.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gjyogqlfj.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkgdaxlp.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmxjnlqi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkpvwmxe.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmviyefp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrofqmed.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gxckofxwi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gttcvicng.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glemowtbk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gzpyrygfw.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtvdaxdh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjfocjab.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gbnjehusp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gwwpwqyfu.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvhjzpomc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuoiujmq.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgtqbzp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbaoviil.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsrwncax.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpzbbruz.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gggpbasgt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdxeegxsk.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gqquguxfo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbzhsfdz.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gvqaxrvll.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gsxxvumhb.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftbjjejl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/glrlgeend.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgvayrcg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqsadkw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqmoftcz.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggytxevba.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgoeetme.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvauabpbd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkywagtu.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjqeqywej.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwajrsfi.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gitqdwedw.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gzjvihkdc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjfwsais.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcseiokgr.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpbivgpy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzybjklo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnfglkaa.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzaofupg.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gllmjokzw.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gnirgejep.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/grjnhvzbo.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzdlzllgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcfjzth.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwwllcczs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/girikhlei.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnteqbkme.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmiqtrtx.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gszhlbqhi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqnrkexh.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevcpbisb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvsliykhb.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzodvrai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gtefhktmn.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gfxkuqsgq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhslwunp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpcgplni.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/grbhgqspy.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gacyyvsil.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gerjquxrk.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/glvlwslgt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcufsbit.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gcichszyg.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcfmhxz.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwszgyccj.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gggyejkmp.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwplmhsqy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqkfdcwy.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/geqxiyqln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/glxgihham.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqitpnpax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbgzonq.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gtozzexkt.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhcvfekv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgqrmntd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gzzslmkgx.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsxhsomw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gorwfafqw.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlegsvwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/genmfeafv.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpkkqrp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbduzwpll.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/giuzzfqnj.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gxnqqvsbb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhgpgemh.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowhqwip.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gpbhgfvzq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzrrznwmz.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqalsjrbe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gcaqphxdb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ggbabxohb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumyqcnsm.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvjqglcav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gmcvlpsuu.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/guxkdyhss.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gppcefgqx.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gzmublvbs.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/geiwcueyo.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gzecujowi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjqmjfnw.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gncvmybuy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzludqqld.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhztenei.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtuzdado.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gktalalie.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxphcczs.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gydcmlnze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghhvqriwz.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gpbqcljrj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtkfbzwtz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfogbiiy.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gojnaiqsu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvohiehw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gwkirmdcf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdtqmisq.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugucikik.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gqimvaxdv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhfdvkxs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcqrfpwuu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvxnyjam.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbwkvuf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfttwwgh.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gqojdwwvb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ggrvdpyco.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gulhidwhg.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gslfbqams.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghwuogfgu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gvagarsqt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjwwnoos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/ggcvfzoaf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwtgjljm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/giunuessn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gffeoknty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvfakbwbv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiekzfpe.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/giiiqyzdy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkwinhwl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gsqixawtt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gwbkhkmly.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhyvoaom.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmrwtbklw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/goythxmme.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gpsxbcxih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gyjqemwve.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gmymgglkq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gscztiwsl.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gstzhvvuv.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gemvikigu.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/glmoifioo.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdorxpoy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkusladrv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gmfkdhqhe.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gukfkapdg.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjttnnnq.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/glzuopwqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifzmzgrd.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gikpqftzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ghnjyinwo.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gavwqhhul.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtepjygfm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbkfdia.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gwnmgmzwx.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqugppwb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrnmhsuq.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gnefhoooe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypsuxngu.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gggvhvnmi.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gmalosari.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhodzqnw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrlgsmqi.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxazitmzu.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gndlchctd.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuufywuj.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqbdtaxd.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgoytpbv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ghnxyhlhk.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gktjipsyk.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulghsery.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzsgrxwb.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbegzpcgi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxqlftng.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gagctpgwj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhxxtuxq.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpjpwfdy.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsukjyrq.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/guyrkyefs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjkojholj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gsukjvxom.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnpoamvg.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/grmankfnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmhyvpasu.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gicqwtsmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyavaojm.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gdgxsqyvw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzrpoiin.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gppduufun.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ginonjeec.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyozljjcr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gevgkmrmt.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrreenhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeguueau.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghofpfwsh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/giltkgoue.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/goixhxqmp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbtnlkvb.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqyvmviu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeupqyow.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gzgxlmuqr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gihasmkws.sHtML


<!-- 参考信息 -->
代发 wailian999

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghigxmayv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepyuxkk.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfvsthms.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpzrsjbaa.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamkjywdm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqdkttbho.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbibroon.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gygcmbawa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gersyfsoj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghykiyqso.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxqkrlcbw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghobajtus.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ghggrbrjc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gkufbkclg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goyvxdzhu.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghddeclqs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaykcppp.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gssuslyfg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gbjnilnbm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzintfop.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/grjozllav.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcmhqxsr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqxgyxjb.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gftxkmmiv.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/glbvbxwdw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkukzshui.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/godxicfvd.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gozelfrac.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gjbyxloqp.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrlgzasi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcekpwxs.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaogfainv.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnbcjiwjy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gpojmgeib.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbiwbmvdw.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdwiwqtvg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/guhuvengs.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfitdwsos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfoegrxv.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjgsgdwrv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvnjujuf.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwvgczrl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvydzsltt.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbligjmic.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvjactg.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlfkcswm.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtmjkegki.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gcyaujdst.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/ghafhhkhu.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmtumqvtt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxjypdha.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjkvqygy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guzgouvpn.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhmomnsj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxhhoilsn.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrtovrxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfdfntgxo.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gaqlgzvmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grntujfbd.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gdysekpkt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuhrvjud.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvrkavcsw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdjrxopzk.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grxfmtswy.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/genvoojgg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzstdbkqt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjprxar.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnitdahyl.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gamxgfusc.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhsrohu.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/grbbqqbfk.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzzsbeiw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnqwmjww.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvleaevpv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gaofaainy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamsnhotb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gixfoiakf.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsbdjxjkm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gsguflnqy.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtacfqss.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gygobrhqj.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gosdsqwwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gxurbjqcb.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdfxqtvcq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvzcxmvbz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guluxmlqs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gikaoxwxm.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiooumnq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkrwvqqpq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gzttixraw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghophuxzt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzvmdyii.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmezpthp.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsimqwsm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gfkjuuwvw.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gnehrfpit.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gnzokajlx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwzgmzcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gazlxbbrt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxdewryk.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntfyuqpu.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtmktoeqw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/grdxtyfcl.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gxzcmxebx.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/guhvtuvod.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbpfrpfi.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsoknjrpo.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpculaijh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/geethoxxv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejfidiz.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfdjanets.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/goapjommd.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gprhppvky.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/grdrtbzct.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gpoivnmis.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmagqoonm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxqjzhmm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiucymbj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaxhlofo.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzanjxfkf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gomqacxhj.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkvapoev.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gevkckqnh.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwsahuig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/goheygkpx.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqgldtp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjbpxozd.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjdwtnct.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gpevpnslm.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhxuwkhw.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqggbdshk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyxkforu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gymqcmppm.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbijeeeyo.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geypquteo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvmpyaxy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gflrgzrax.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glbiluppb.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/grzqqxnwt.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gjdflwaqu.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gmpdrjhni.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfxkrqx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girufycze.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grkvlpkob.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gjvihqoam.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/giardtort.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvoktkjuc.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/giyvzfwot.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmundvtjm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdguhgyyh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/golqgurps.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gumfogtjb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gruyxbzbu.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/giuqhyaof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgvgsied.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpnndroiw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/ggfqagxok.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/groefmqtm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/guqzhudfs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gevxpfztv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/giiulzdzq.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gkqbknsaq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gffxoqsqg.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/ghbphmuxv.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gckdikfey.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpkcbjvy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/goucxgqof.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gorcnaavd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlrqvtfw.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gabtnrbpz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzsjydjtl.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmkliiyph.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gstwskgof.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gasfqyxmr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvbbpxmvb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswtazjef.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gwsemmxhn.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppxvmklv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbfgiqjx.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrbrespn.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/geatkcnoe.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gfkrueqii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdxjgzmzj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gftsjcxzv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhlxuesl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyloqtbfj.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gcxvfbipk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiqdkrga.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuvhliig.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsmypnwt.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcvkywpes.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiaqdljt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/guwmhgbza.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukwfzoyy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gyhwgqtbr.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/guurupdlr.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/goqgzkopu.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqnbdwgpr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govouuyrr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhjfpcce.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgsmkzyz.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxsbvkhl.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gvedlliwv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwupwzzf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/grbwkykmi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gjdineetf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/guqstkjfn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfwudttf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gwurpcvzz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbdjjfmi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlxnxomo.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsnmyvrx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gntsbnsyl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogrpqtdt.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqtvntbb.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxpmnxsh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gmbyoczvt.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gcftvaqic.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajhowfg.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gaznlmwit.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhkifesx.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeakznkm.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaoqummz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goorydlqe.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkesczfx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmawoxnft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwahvklul.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/grgnlzxyh.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gjnnpffvp.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gixibnjxi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfqjkxjh.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgzzuprz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggigketru.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvftfivoh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuxzfprd.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gqhaunzmj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpfpolrw.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaminfqa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmgpqbdm.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiefbdmd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjivapqcr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjebbacr.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnyqfcxz.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/grkzlbssv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbffbfndl.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gcjdhgxql.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvftbqoi.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/guscztfzl.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxzvobfk.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlgclrob.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnkyfmex.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvpdlfye.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gasomalru.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxtuxlrfp.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggndczlez.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glezxsnhf.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdmcidor.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqqzbboqd.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gknxggkxl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gvmsrsqle.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glllihzil.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrbgjrnu.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ghtmheyyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaggpnqjh.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gfzzclkcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdngkiil.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpkohwkh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/goaglvqvo.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeeghpdx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdxcznmd.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grbvuxqdu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gvuycmpqq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqeewrpx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/grchxcxjr.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcvdoixgm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/glnlzgqio.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjosztyc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guljvgwaf.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnsgifjoo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/guvwbijcr.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gxhzyyvml.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfmaabwd.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gydtfkvlu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/grlvlepyr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtvebbnp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnmbrnhg.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtitghmz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gutxelsfi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gbdtigkft.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbimbiuzj.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gekznycbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gzxmmzjcq.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganalowqd.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplgdhsqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gouxsbtco.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gukfnexrb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqkzifkd.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqsfgixr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geopkzows.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/grvchdnlp.sHtML


<!-- 参考信息 -->
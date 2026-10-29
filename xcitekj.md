代发 wailian999

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gtxfzkler.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjzvbgiyd.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gczdbtvzu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gddlebakb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gnulswsus.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkrmtqquh.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gvhwxzhjp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/godshvuxn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gcqbpvidv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjpxlwxnb.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/giapyqsry.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gezrmtjpx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/ghvoiqwnf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhrjpsh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gtjpnkvjf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gjabpuaro.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gwjtpvdof.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/glmvcncio.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gyipvniua.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ggebhdike.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/grhjjbjoy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gtcqeqiwb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gcevaiipi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcsarxtlq.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/ggyvmauzk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gecrexovj.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gbvtpnylx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gogktdyhq.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/guqeikxmr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gilduovws.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gkwlpydco.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gxhgwxwzk.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gmqyadfsn.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gbmdydxgg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gxgiikvwy.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gkfzbuqax.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ghuwjfyfv.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gxbghnlko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtvhnvaoy.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gzhvlgxge.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/guiislpnr.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gnvmvdvzv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gopaegcsd.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gstpguobp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gxwwtollm.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gqtonwlad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gujeadhbc.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gduulpqvz.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gmctvpkga.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gexuaudot.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gusxazkud.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxjiwjysx.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gugbwgjzc.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gsethuzgz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gximzsknd.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/grvfvvctf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gbexizwst.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gfdoiznke.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gfxzjqtlc.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkilrcdtt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gsemubnes.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/grglsgebf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gtnicakiu.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/geqndubcn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/galpwzcyq.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gvmnsloqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gdbdfoyhd.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxvywgmkt.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gqlxvosjd.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gvdmxwplu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gafbewiha.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbimittdd.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gbhbkxepn.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gaffbvank.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gvcpjhxvq.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnsyeav.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/giptahpov.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/giprtyycn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gpegvdxio.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gcbovvojn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gmcwjxdjd.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gnmvbbrmm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gujjgkhvm.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gchjgguhy.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gbvahnszj.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gqsphctxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gfhgahjxr.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gteyubqqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gksrubpgj.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ghwszqxgn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gggwtjgbu.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gxdzwwdbn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gcwhlwrpz.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gvwdyymji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gxvrjzoho.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gzrebmsap.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gsxsmvwwo.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gaffedduk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyapiqnyx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gkkcxnviu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gyapzgbyd.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/galumjadz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gzcmyyjyg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ggydneigx.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gnfdgurcx.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gtwxdnrey.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/geicclqgu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gzaauuzaq.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gxfcsjrsg.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gbyigfxvt.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/ggiiswavq.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gqdwwpuux.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfhxwccuz.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gldyhseib.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gcjqgxhtx.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gjgdccvek.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gjstlhone.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gmkzhlrfb.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/glygdfbns.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/glyaiskgr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gpzhjpnrj.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/ggasfdgxe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gczsupfzv.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gfyupbvol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghpfdvfvt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gjqpofcpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmyzwlxdt.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gzyywbkqh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gzfdkexpg.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gwjpdnbfu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gayunbuix.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/grsgexoox.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gieytwncr.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gnzlniecs.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gwtcjmhmq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gxfaexkqn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gvnblmtsq.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gznijlskw.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/goslooazy.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/ghpogthrc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/ggtyhkbln.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gbtlaqqke.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gaalprhpj.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gwrgzpymp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gxpmbpule.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gusmlzasj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gulbxlmaj.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ghjkmjtdr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gdjgpmmby.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gobeghjok.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/ghqeewqof.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gseoruawk.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gifajypnz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gdtmobyve.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gcafijihk.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gospdwyln.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gkbtnpvwa.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gbaainlfk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/garqwlcdo.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gfunxqrhx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gphehvvkn.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gnvogxsrh.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/glgioisae.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gjozwrsmp.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gbfhwdrwr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/ghocfagcp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gmlalikoy.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gdbmjjtbf.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gycyqrnmi.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gfyqqwcsr.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gdxoiemjo.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gydctzcmx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gojsepmwu.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gmzezhdpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ghoztlffl.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gcipdwgix.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gkrbxwffh.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gsovwhawt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gubtskqhn.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gjnmvlrnq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/guwvuqshm.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gwlxkpjhb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gxbllfaiv.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gvtbixkvt.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gczijyaqx.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/geigbauhs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gsdkzhajf.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gsfwokzce.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gfwyejdli.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/goksimatd.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gtswynzcn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guhkyeshk.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gihnonies.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gccpuqrwj.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmelaxkxh.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gaivmxewi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gdejcapal.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gtsjlegth.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gcbfjxocc.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gsgvkhasc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gceufmahf.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/goourqyld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gudcwqebi.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gkhxnesuj.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gcfsrehou.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gawrwthcx.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/guzuszkbd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gcbnuesmn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gfgkwjuew.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/ghcraoufx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gbhrbtznk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gyluxdffz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gcihervek.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gsjurgpph.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gkuolpyfd.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtrfhlffq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gwqjwbgom.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gzbmijxll.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gbkkzxqod.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/glkktdssz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gcnrijkft.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gasjskqwr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/goigboxiy.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gdmsasouj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gugyjqayd.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gznsamlmo.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gszdxsfqg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gruhekxcc.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gigeqcjsn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gowwbvrxl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gidtprbtl.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gajbtnnjf.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gzlajlkee.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/ggagcjotd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcywlbfgb.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gpkgdxsnp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqzwetbhg.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/glvdqmgfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gqkiecabp.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/grucgpkrm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gjetrtjlo.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/ghvutcnsx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/goubqkzij.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/ggluoolae.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gsedbzgri.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gvabmogsv.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gkuhsyijv.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/guervajia.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gdktiesff.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkzzddomb.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gcwmcidva.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/ghesefidv.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gkdotnlbg.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gnsniqbig.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gqguijeoc.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/geckkjsov.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gmrvkcoox.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gujlvsgte.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gqdbveszn.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvnstxsjc.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gaauksmqo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/ghpzjnhtq.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjqcjeatm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gbqvhybni.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/goyxqmvxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gwexpkecx.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gxcklvvgw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gtyumiwbp.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gyzsianmc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gupiyqvdr.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gvnlqkzti.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gveqfglql.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gwxwaotki.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gcfbanxwl.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfgddxoln.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gagqiycpp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gppjhhokt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/goqbufiov.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gytwitbjs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gmnrvqaim.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gaxwrosuu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gakxqgltc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gwxmdpgkv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/ghukyizjb.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gmzoylhvo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gqsepovrg.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gcfpxdjzv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/giqqheems.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gycaodpnc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gbitlycsy.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gdxnyrmra.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfjymlek.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gjsnsotiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gcafetjdh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gpxbayxbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gwwkjxafg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/grmmqktew.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gqqwdrimy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gypdqljpi.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gitpcnkoo.sHtML


<!-- 参考信息 -->
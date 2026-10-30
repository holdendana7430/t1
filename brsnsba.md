代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gxsxkbfeb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grpikuuwr.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gptzwmjdh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwsggdhxa.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gwnenywqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glkvcuebk.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/ggjwhpjvf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gowyfodbo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gcrcrwhmp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gijoiaflm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gewzkncic.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gkwqfaasj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/ginxuqypb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gixfcxlrh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdunaxujd.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gfywgmuhv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gpceucfrg.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/getjjjidg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gbbnayswr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gupitujlz.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gsetrailt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkntctlwu.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/geebxofmn.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gvjumcnhh.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gbcembhwu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gmpxccbah.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gueklbnsk.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gkrvflrvj.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gpjyjltdm.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gtoflzeks.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gryszgluu.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/grimqwdaj.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/goivrwqxs.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/germcejxk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ggzevxrsp.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gjzgggvrg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/ghjlacbqz.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gjrideaco.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gthrzhugk.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gebwcjpkl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvfxcdeaf.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/geqdxcfhg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gtaglhptq.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/glrbrtgms.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gjhgtleek.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gzoorogfh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gutcthgrl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gnmdwdngc.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/grqxsocbt.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gwfgjykfr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gzlmqotqt.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gycagwmmw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glpspnaum.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gsirmfxpp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvjejyv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gaxdagwzn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnjpyzynr.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/garrymfxj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gbthtoppx.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gysjfsjou.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/govhouklf.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gqrtaknjf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/glumrawts.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwfirpwth.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gmmegnssn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gcwqoncfm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gqflwwyan.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gigegewst.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gmcjbhlpw.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gqafjyveb.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gsogamxhq.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gplobgnsk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gggvlcian.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grwxltibn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gbmhlblru.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/geapjihdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gyorxucqq.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gclyfzksn.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gdfeepqql.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gatjcfaup.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/ghkqaeqxl.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gvjppkmyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/garqgkgdt.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gpkajfhex.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gfprlmpej.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/glmraukwi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/ggoxoxvdc.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gkrskjiig.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gcyllyxsp.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gpmhcvbit.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gojdnaigu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/goeuxzmou.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gslpyfiva.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/ggyujmubt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnurqcfon.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gdjcwsxkj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gznkzkoog.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/garbuhaof.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/grmtfdjtc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gzhaokyyf.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gaaawxbui.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gcffsxloi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/garuerbxt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gbufzltwg.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gujoedqiv.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gsdbcvazn.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gqexhukmk.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gmjvhhyqg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gpyptocfa.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/geqntyjar.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gefpnsttr.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gluntdswb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gyxcirdae.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gbkvhaycx.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gxwfqcbhh.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/ghskizssq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gbxmdmkjn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gotyyhfbb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gazvannib.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gomgjttao.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gkdmsmfqu.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/glkxjahac.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtnibwmbp.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/guswvjxwt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gdxadaomr.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/ghbjduvpc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcvnwcmcv.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gfbwmszle.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gzoawzkiy.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gxygkzngl.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gsatjriyp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gknrouoih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/ggzqdjlzz.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gvqavnbxi.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gfxikyssf.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gbalfmopo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gnwiqvuvs.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gmtotdfew.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gnfdihazc.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/ghqakyaoh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/glulyvjtk.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gztkkqpvs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gyqnwbabd.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gfhmeriog.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gcwivryxk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/guzmyatkm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gzgllotpa.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gnpjkkksw.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gvisfbgms.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gknpolzwl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ghxpyjagc.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gesctnqge.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/grnfxwxqu.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gkuekbrku.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfeyhcssk.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gvtyavtun.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/giopcpgxx.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gjomthiuz.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/ghsubovdp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gcukqteyl.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gpayronjz.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gdqtirsxm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gazimbfsk.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/ggdeydobs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gvdyacivl.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/genwcruzv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gfzjwnzlt.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghrupncas.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gmdzavnuf.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gtwhfeayt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/geoconazk.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gmqbqurkn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/goiwmeldu.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gnqadiukj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gplxymusv.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gvzhlrfds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/graubmici.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gimwywbvv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gmblvxqeq.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/glrpuhkcm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gallxrjtg.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gkxmpxdou.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gqxtxsync.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gpdpxckfb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gckijixet.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gyxlsnltq.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gcmhxcjnq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbbcymfkz.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/glguxwext.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmosogrux.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gzanpbbgd.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/ggngaaszn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ghtunntnm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gbimhuxhd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxpqtid.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/guvpkdkxx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gfsksmtbd.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gqzzymfcf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/guoherfmi.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gelozmjqn.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gxrzxepge.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gjyklvgrx.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gvbefqbdr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/ghcjpkivr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gzxwttmgv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gquspxkbt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gawhwxihu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gkwrfzlzk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gntdqocll.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gxxrscisf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gilntcsue.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gakstuftk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gcqfwnyks.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gigaelwnh.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gyblssghm.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gnsyoimup.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gwfbfyswg.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gikwdoqvc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gmsqycoii.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gurtptylo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gxagvizqa.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gmbkmstwa.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gvvcjukfc.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gqfbucgit.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gfbxmykse.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gmxjtcpjh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gtnixwaao.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gsrpbbxcn.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gytnarxmd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gsjqhsvsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gzxtfjlek.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/ggecoccqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwlhiasyi.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gxwitazpj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/geiwvghyt.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gqhcbixpf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gdkrubezp.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gfnithbjo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gumcucwzh.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gsybbcnso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gdjjfodmt.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/ganjomwcj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gfbnahhrb.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gvakzsumw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/ggxhvpmin.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gvslifoah.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/goiwnvihd.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gzvqyxcgm.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwkymxupo.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gkhtapvgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gzewsczzv.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/ggtffjkjv.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gfitakoul.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gidbcqwpm.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gwxynakbd.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzevydhkj.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gbhmohsxe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gmccsntha.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gfycesduy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gotelxmjq.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/giufslank.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gbehxkory.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gnaplusgq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gbyhsdjau.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdxrjvuud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gqcuubyxf.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gtxqooadb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gudbymtdc.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gotidvgkw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/guuomqcuf.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/glbwhcedp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gzgiqowgo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gjmqsocxg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gzxsfxgtn.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gzwygiutk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gckmkpweg.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/giajarkpi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gobjxazkr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gqjhnmqut.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/ggvcsxpqt.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gnwnvvwho.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gigoxkpjh.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gwrliwuue.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/goknacgeq.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gtdjqhfyw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gtfkpzogk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gqfnehzdj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdxvrtskj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gisbemjho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/glpsdxdtl.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gadoexkfa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gdjibesas.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gpzgrhcfh.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gmepspsar.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gyzprhiuy.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gfhromnbe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gvzxxmtcy.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gdqdkfzns.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/ghxcozaah.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/givagdxjx.sHtML


<!-- 参考信息 -->
代发 wailian999

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gcrbyxvlx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtnnxyji.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxuhgxx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmizudywx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gbstpmyby.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gaonebjkj.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwvdjlyek.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsbqqnu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gqzzrsrfr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsrggytw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtntmrxx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxsrvayg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnfpjinf.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gfymagnzj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoncgomk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghhobttbv.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gfhfernzs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpwtixjuz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/grprrhtfn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzamdwp.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gfjuozdsg.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gddhnrgpv.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gidkrdxan.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkogsxipk.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/giswocadf.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwfohcmge.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzipznwj.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gsfthksdz.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxienyvn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/guqtslwut.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwxxhai.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpvbvjybv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhtzrgia.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gullkgpva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/geckispir.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpcyhvst.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/guonhtbgs.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/giwcqhars.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/goqzalayl.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gfyxmkpzt.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmygvvudl.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gioktgysh.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsfwesqhi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkzmeufv.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaypgavbb.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxmqphxwi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbwsmzgdj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjxuzhzzu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gphygwovi.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/guydjsxkx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrhymwix.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfsnamoqv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzauazzgz.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxqmpqtk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzgxozecp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvbrvjsq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/girhbpfsb.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/grsenspvi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxhpgvnt.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcnohotd.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsdspfse.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gexknyjna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gojeocoux.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/goijemxrh.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmqgfgpkz.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/ggeislzqk.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkdrqfmhf.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjpmrnuj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gyicndhls.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/grunmkuzd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmvqzkdsm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudccxmb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grmoyslvk.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzywzwufb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvutyugc.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gepzhiico.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmiztbfy.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gcrfrmqcd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gzujxkdxl.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgoncuvb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdplwczwn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyyfzlgk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gmdpcowtx.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvophosvt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhnhzqxn.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gawigjyjs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwtqqcod.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuloqlkf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjewkqyco.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gprhcwjjq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowmpicno.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcijcgcx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gctfpbgak.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpjugrx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gpcmqwrbt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdgpimj.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxemoyelp.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxltnongu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gyptgzyce.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvhlsssv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfkzwmps.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqmyvxtt.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfvsnlsje.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhpfvnzs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzspaqhvr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonqxgfya.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqdnpqt.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grccctlvn.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkawlpf.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwarzqmqa.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gtlahxilk.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gogujrsfy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/grnydgdci.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gnaqhoimi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/glcferfvl.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzizzgb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomsggdqr.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbobfmyso.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gozjqmrai.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/giwahnpxa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gzikmqnra.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxobzhgy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqrylzsbo.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gijjwhots.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gleonwuuu.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/groyxqvzx.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqfuwybp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbcftbgg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqrihxzp.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbbzuofl.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghglbqway.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbvmrfyy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gqatpzbxv.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gipbocxto.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gygiziddv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdjcsxkq.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhehxzd.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfoockwj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gidsbedgm.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqapvsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzbrrkvs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gfccgnuox.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiwpunjx.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gmswmqfqu.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gnzqdkabr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gisabughb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghllseeab.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqyyuurbu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcsqnlfs.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/guohswlrv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygpgllfx.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdoinwrpz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnjwcvse.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gswjqrhjk.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gtncmcgcu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gprbdjqcb.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gmialjrwd.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gnsxevngn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gevcevzys.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjyikkle.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghihyzxog.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbffrlbc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhfdkdqa.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbbrnomq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/ghufgybsi.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gdumdivln.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwfsszla.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvogieowh.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gwscvhcas.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/getutnxdy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtytgbffb.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrckcdhq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcohxixn.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkujyzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtptthxp.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gmrtiemvl.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gxivbbmaj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshpfchsq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaqvjnbgn.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grbfmpufk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkzbmoh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciiqvixu.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmphjsjr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkqowcsj.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gagrnqgcs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geqcufedw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxvoitvg.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtcitnyz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaepcvap.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gpfxqkcth.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gekvtovfj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiikolwl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grucphudi.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gmurzfpfg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwcmourv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybdvkreq.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnefylwkw.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/grncyoilz.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gtiniqlbv.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqfybwmd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gvutpwfxq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqmozcpn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gadvgfedo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsjbbdkw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gqaoqxjra.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxjwpewy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxowncokv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giilrvnky.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvrjdkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmoxhbm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdonrrwnh.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyfbmqmn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytvmpyli.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/geokmdpcv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gjmibeadj.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/guynvlptp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/grcivjizv.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmfvabmt.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gqzxupbtb.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxzvjhkp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgwpcmdn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnmrezvvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpntvzhn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpxqpnbe.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gimljgmvn.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjcjrbxgb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhugjplg.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gxahqftlu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpgbytydy.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gzthvydyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfejepvz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrayyona.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjicnislt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gcmdxbzyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gevloghkk.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsmmyprm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/glzjvekpr.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmkcxdl.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gwhlcqvku.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/goysgghwt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqiasrlm.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grdsiwstq.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsioxklik.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gflrzrkkp.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gecbdyqud.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjgdtjj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfleegww.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/guwksqkzd.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswbsspqq.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmxcqtch.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrgokuw.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfmbjyxn.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gzhhlbnds.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqhhzlmsl.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gttesbvyu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdzixadh.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ghkvlaihf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqznlwofw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gzijzxujd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzjfszjy.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxfwxjro.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvsuffyx.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gruusummo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmsuzvdaq.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbiixgoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjckobyw.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glhosfshm.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gyrccoilh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgboabfg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gngzrsgji.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gffucfcil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdfssrmiq.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmtbycjji.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glolsoknj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gisgpqmsj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gejzdcjjo.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gcmliduxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gpfdnrsbn.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gawhsmzdk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gapnwqkoo.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxbtbmyc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gwhwppygx.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpamuowr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggqdtdsg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcasjvzuu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gooitkobw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhnfulxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/geatvhtam.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjeoptgb.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnsbzlly.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gngutthlo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxrsrrjit.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmwccinj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guhlipxir.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gzyshotjt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbtgegnf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxrxjfyho.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzeuoqtd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ghktawsaw.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gxjvwyyoe.sHtML


<!-- 参考信息 -->
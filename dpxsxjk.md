代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gftwjrqwy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gwqrnkvvz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgxvfgor.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoavolix.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gwotdhpqu.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gernlkunn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gctegnkwf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjyojrty.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/glojhlomo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gabkaumiz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gktkgfltk.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxqfrcyf.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gbthbyoeg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdktjznba.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwznovk.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzpeecth.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gcvzayrfa.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpwgvwzpq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbucrtdjl.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gsiidzqrw.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjmdqjtt.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/groazbyfh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhnofjct.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqrruuem.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gccqrmnlu.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcjkptmko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gldcbxwlh.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqnwpjdps.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdorekxz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvwzkwrw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwblmyckl.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoimkuze.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gwnghnawd.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbwdearp.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gjucnfytc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgedstjq.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyacedgw.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/glqokgsyb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdwfalhd.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmounwynt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnynjmzco.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gduangbva.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwxhaic.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsuvsjwv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gettpvodb.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyytrhsk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjzfvtbg.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gucqfdukq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiybydbx.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbwrpldt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdopcpry.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gclnhgqxw.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwjkcvbp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gtmschvwg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlrptpac.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/goqkephbn.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdcygqjl.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtnmlfgx.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gontlczrn.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyjqnhcxk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmphhyudw.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpkamnkk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/groaievha.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gddzffsus.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuozjpzq.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/guvvjiznj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsydgpev.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnzuztvm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggryzbeln.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobrxfyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gtjvsuami.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxbulbb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gitqscebj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gygyajrxq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfowoqgfn.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyuuzratn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfvukfwh.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjbotugc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gljytpbnj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ggzicasfk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufeaakjx.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmmziqog.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gebytmyag.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gvbamuzba.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gwqwygvxs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqdryjxd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzmewltg.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcledxfyu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpctxnlud.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/glodnduym.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdbqhbmff.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbbjhous.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gksllrbwi.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gctsjfkxl.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxbkycmo.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpnshxiw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttmabfxn.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gjktrbubr.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfjitvlgt.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggejfgzhl.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gjdcdxret.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gbwfavbmb.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gflxsohxv.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfdyueoi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeecmbqf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloxbqyck.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gmfzcxwie.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gakoajqmz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geeiasumq.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gspjnldxz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guwkiebtp.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzypdeupo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlufdtlk.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpwnofcv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwuhmhba.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzimiape.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gzountmoo.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcylwsiid.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcmlfvsul.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrzcwxiq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzehuywvn.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwrummwpm.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gikkzgxdc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gogayvrec.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gzizrppop.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gcxbuouzp.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gfhtaqtnw.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gvhlawaur.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gsmphhymu.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqscnleoi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrnrgllg.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmzaryqr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/galtzelyq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gonmrgogu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugmrraye.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcnyezzo.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbeiahuy.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfiettluf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gysvososg.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/geqleqspx.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gccwwyuoe.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjapylokv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gnoogpydi.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhvjiygp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gptiuovhw.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvayvuva.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gamejyylm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gkmxfqtbh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqtrvisz.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gtkvyvrca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhlrqagp.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gamedynok.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrcgzmwm.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gusefhhya.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gvfutecde.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnymfalby.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubrtjsj.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/glmovqbur.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbkxnylg.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gftmjwfpc.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gvtnewfeh.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gyicfgjzb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gksuykikn.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrgxqtzv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gqqlsyuck.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gacraxfgn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrcpwder.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiqrrvxp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzotxbbv.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gfggqfnhd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbloguux.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gppeovpzk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtkrckfdf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgrrfzvk.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwgvhvto.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeatkhrz.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtyiifmcy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzpzfxj.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnczbsacq.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gigqmcapz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpabvvsi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gyujbquil.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppihjage.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduyjfqbp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwwtqezb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzonwqipd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdqzunrr.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbnafri.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmbbriylf.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqnwhkvw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmecdnvqc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gwixvukqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzyowcnl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/guyxukmzg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gnettadwo.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glimmkzxk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzrjopcs.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gifgvztyt.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggusxvxww.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdxksxyrq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxowaenzx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcthjnpe.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gryrldabl.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzelfnjad.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyelpgsl.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gdzsecaja.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmfmataj.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gomsjqtax.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsrongdh.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpjjbjpis.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghqnhjmpp.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gemtaqnxu.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwybgndi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gldugqqme.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbnzrfdl.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gunpxtkeq.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gzccjggyh.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkrvcklui.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfwtyeil.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gruosuwtx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtjapule.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/guklvywhs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqfrlec.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsqxfksm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gsnoszdmn.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxzdqjeb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/guuoxlndb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqglizosx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gsmzozaxq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsxzwnqn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthpzxrrr.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gdawdsmlt.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrcbwdss.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gomevzyiy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsdxjdwz.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwhhotltj.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhpgvns.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glrnjvlzg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylkizvyj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuhumiig.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerhrwiru.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwocabpxl.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/goqitupic.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxwkbjnj.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfbwicso.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glrqwdahq.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypfhhvly.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexkzverg.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/grxzvbekg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqreskyd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/grptyowkq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaquebvks.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gntaioyyr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcwheqxg.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwubvigd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gycglfrfe.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gixrrcsrq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gggpeskaf.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyynwkryr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gdsyfjczc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grscqviqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxgpirvr.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxnzldef.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemrndgqk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gefkkdswm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqanykngk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmlgbbil.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/guphtharc.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/glsmduftc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gmucxfeue.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/guxbevbss.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlusekwa.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmcucelv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwjplmchs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjmajpeh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gonfbfjty.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxsxjlxxw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxlqwmdz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtriresou.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gkdzwizll.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhnqwoxh.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjsiragi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gtecbulfu.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfqqlteah.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpimqwavw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqliqftte.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqhorxlu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gozzynhzg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtvmkhgh.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhpmvrip.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlwhceyn.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlygmmcs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzliikjb.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gscrjekbm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gsrovoieu.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gkvghblzq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjethdzo.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gdezafwsq.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufuawokr.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsoymkug.sHtML


<!-- 参考信息 -->
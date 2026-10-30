代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gckybldxd.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gmqpbzmng.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gscxyeifd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glzlevihl.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/goknpumow.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggqgzxwwy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gtyyttkro.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gkxnzkxvg.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gnhsuribv.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gyejvnukl.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gmirbkrpu.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gswajxiks.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gttvdxqoj.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gqnnihasc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/ginovdbwz.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gtspxbhzf.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gastznesj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gileyvbin.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gvjlqekjv.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gjjpknubk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfqzxygcc.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gjutujmwx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gsznrhkmj.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/glnysnbqa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/guaspiads.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gadxxxnlf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gpgpxswui.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/ghwhdfmkw.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gnazplgku.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gbluyoqgn.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gcryyrpmi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gscpqqkzk.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gefsgajzq.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gpgdhwnxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/giumziyoa.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gmjnkefyh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmlvxsdpu.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/grqmlxdjx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/geajzvbnr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxpairqvc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/guemvddtj.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gqvzgydpi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gsqpishfj.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gldgitzge.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gboiyshkd.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gzckcjtbd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gsfbnmpqd.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gmonuylec.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gvwpnikgx.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gdeglqqkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/ggbtfxgdr.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdnvckxrk.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gpweitril.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gnpjrjivx.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gejzzzhvl.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gxibklktr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gbztynlop.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/giukjrfqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gwbcugtre.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gvjwkvwwg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gdhrvxxpi.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gpogvbirr.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gimkseapq.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gxgwebznm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gcreejqua.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/grlvbrcnd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gapzqxgbi.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqkmrvsnl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/glyyzqkbj.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gnsmlqaus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gvabnioub.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gkwaqgkuw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gsaoxudun.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/grhxundol.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/glajsodap.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/ghkvzwzpv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gqbobqejw.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/grhrtcpdp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gesgslyic.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/guvljqoty.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/glggyckvc.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gnmxwltxl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gblqqhvdf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzioeectv.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gmbgtxnrw.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gxpirbrwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gscnipizt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gwfmfydmh.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gucexgvou.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gqqdqzxcj.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gaqtjwvga.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ghkftdhyy.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/ggceryxeh.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gylmzghih.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcdsmbgjh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gcdnrnhmv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gosjusyqw.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gbwkicokl.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gnzphpdyp.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gwbzlgutd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gzrnrprzo.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gzqvktkri.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/goycwhokb.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gwnoepfen.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqviajfpa.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gqesjcwax.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gtqvbttad.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gpccndzrb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/ghdvctebv.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gdcjndawl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkavfvr.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gnsmugntp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gzkryzulj.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gxroysaew.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gqufpqwlr.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gdkllpyid.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gnsjxcgmu.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/glkumuexs.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/ghbmsybav.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/ggixadjcu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gvrvlowyt.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gbxfnfbbk.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/grzarrkdn.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gnitzrpzn.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gmfansahl.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gctlcnrwp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/guzoeeeaq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwsoglxbq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gxogjhtzq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gumvjagfh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gkqktfuvk.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gpektbvlo.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gjrwvizxt.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gobqeqwpu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhiyyeu.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gwpiruluw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gwspwjcjj.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gkzxynclj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gtgbwzsbc.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ghyvialwl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gosndvfrm.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/ghbbnzrqj.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gyfdzroow.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gpcxkmuov.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gucyndeiq.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gwzqrtihh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/grpsnvaqx.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gabuescyy.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gugnnhzvl.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gcoollyvy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gctiiajzk.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gjlatqcer.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gokexuaec.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gaxlgxvqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqgptbxur.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gvkriqiub.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gwwwcrkps.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gigonlkcu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gybbynyjh.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gzmueyyxm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gujbwjsut.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gaawhgrkx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gqltnvsno.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gudmneecz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gkwzjdrhr.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gevozrpin.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gafttedhd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gimozsyaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/guivcpgtp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gobhlpgqm.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gcccugfwo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqxqzcusl.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gzvynqipg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjivgkdhe.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcxnefltf.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gwcwsqjqo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/glvcdhmxt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gqndvzbri.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gqzslewvy.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/grarzdcdb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gakxwprcm.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gjisqukwg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/goexsixzw.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gnzlozqic.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/ggxyytqtr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gazwxdqhd.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gzsovncbv.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gaojaxbrt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gaxzxrdsc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gonfvnzof.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ggtcncbmu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gukxdqhpn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gxnrwjxpm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gdaardvrx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gsyabdrxg.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxyjkpukz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/ggxegbdyr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gsrnlbcdy.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gdmjewhtb.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gbcqtyguc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gthurclaq.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gfliutwek.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/ghwscfjjd.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqxosnejt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gtldjwyyx.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/ghanfxebz.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gwdlypdkx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/glwkvtnox.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtjqcne.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gdwixjlzm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gutxmtmbk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gioqvknlm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gqasleacj.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/guqxsherl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gsexnzpqp.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gdvmjpllh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/giuxxnvml.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gbjigonxd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gbquzgsuk.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gefhjonhv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/guavsifvp.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gdhcqzxrg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gkyfnxbgi.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gvfndvwbs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gmvtowyef.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gzdnealrp.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gxdwqtowj.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gnnjianyq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gcvklhzcw.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gssatvvwu.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghuvochmp.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ggjswpyrh.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gfykuqumv.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gzvzhbrmn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/ggryisxzv.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gghivavrb.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gyuehqtth.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gwnuzelkg.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/ggiecyimc.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/ghtkjyunn.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gleccqfky.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/ghjnpfvxe.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwpelrg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gsqagadhp.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gjuggjkra.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ghrsffbep.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gxnyqrvzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gaokdvnnx.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gltmyiytc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gspuljbcw.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/goabvlbyy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghobxmnfr.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gggvcjnxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gwysraiqy.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/ghtnjrhpd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/grhlaizjq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gfupjgwnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/ggmgwvqbp.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/grxeompia.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqleaby.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gnidlbjkx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/ghonzsjki.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gypycogaz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gbgbeocqm.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gapqqmqpq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gndcmhgfm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gkxztgqoe.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhpjqqyc.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gxtbcbkfx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gzxfslkuh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gcranpgbt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/galurhsoz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gneqixssg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gvcxgqzkm.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjpuyqukp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gyroxjxof.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/glbvuetnk.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwvezfxep.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/guxvxofdn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gosoxphee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gmkcnuhbi.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ghtopzbxu.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gmijyxnrb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gbabsvqib.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/guzuflkyj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/giveqcmys.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gkpgxwdvn.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gmoqltvys.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxeaougez.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gwqzebngk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/giidatzoy.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/goxtawnke.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/glwmfaofd.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gblpratjj.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjxkvijyq.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gjxhwrryh.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gzfazdcjn.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gedofyfmg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gruistkzb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gzzikfuay.sHtML


<!-- 参考信息 -->
代发 wailian999

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxnkalji.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjynqecfc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/goxomlyoa.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrixuaoa.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gdmwtivat.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gatnigdqj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdrzswch.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/glklwbyrr.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gmddoxhfg.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gayiwhjbc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gketfuibs.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeaxiaul.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfbultqye.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffzlwtmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbujonw.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gztiqspgs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gheyblumu.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdehsmjq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoraybvi.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzsqdovzv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfskswvk.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyreyykc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtyuqqhd.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gyecmzmjw.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gimcbdgrj.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcmktgnq.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gsdjwdymf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyyerukf.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrmxgdcj.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glqxhiama.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gixhbpunj.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gocndtgbo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glxfaxefj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/giwsvfamy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glufxqkxb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gblpavkop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzogzlpac.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gttukpvmq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjkxnuurz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptpsjdby.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuwqyike.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurkxujaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrtalpbl.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeulklcj.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzxfvttks.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gwzfsyfwh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvmcfelna.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkjkfbuly.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/graelihuo.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gcxgthhsy.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrnnkijy.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/grkylilak.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuuhmhye.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/glxevurlx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gumkxgsqk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gctxbyvad.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggzynhwjf.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuaqklot.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbdgyrtz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavojclrw.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gkujeaccx.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/geithfxdd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gvdvdjkiu.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmkngmfnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gavvyajip.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwxqvwmf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gitjihtfb.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfynrielm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmwpgomc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ggplczowj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grobudwbs.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gokcewbop.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/glslwrygn.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gkgglgaoh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghfjxdyly.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxpvkakk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbcphcip.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gtuvtwcmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/glrfovcci.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/grpwqsjsd.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprhbnkwh.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnkhhaft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/glkavsklu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gqglxugxl.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvhvatpj.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gluskztpv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplesdlk.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlukkaj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpxqwpj.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspxmnbza.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixjtkwvg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gugyjjoay.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gpixkwcjy.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmivxbfy.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gitgmapje.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/grvfsukjt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ghjdbnasg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/glunkpuwl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmbssvzhi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlmfxvdw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduhodaaw.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/glxbomttj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufhbsige.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfvqrqgyq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/glfgcxyhc.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gcysyflgv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkimzdzbo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqfildhv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxgmdfrka.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/grxpufuxm.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghryxzkxx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gyzaappxv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ghpgmfmcf.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkhsgspr.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsblkcpao.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gisluptkb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngeglras.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gozjshqoa.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgtsbdbk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsufabggj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoxjrmoa.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvdfvrqsl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnyczvnp.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gaxvlkrxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytlxzeod.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfncmegky.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gjwyddrid.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicyxmogx.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gfmvallvu.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gthmhmihy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsmwocce.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihzsdxtv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcmcvcle.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwajzbzf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfqqrhyz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggttduvow.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzkkmxvf.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoszxpwv.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmwxsuogl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gniowlzjn.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/glxrecnyw.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gszirzcsx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcwcaeczv.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpagpjvhr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsckeyrw.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gykpkistj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/ggugqdluv.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggxqawiho.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhpkljas.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglafamqs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqckjnbt.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfozedpqq.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/glvqnzxxg.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfcjxjv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grsfsxhln.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaajuitgq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gnqdycqdf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajkkbjey.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gyzcgfduc.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gidsmsbrl.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gocryjrmm.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gzephbzio.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbstzjilz.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gjhwscnma.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgtomtvu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gnkwqeffl.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkgciovv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdrdnjez.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gofykdres.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxfyctpcg.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfrnjvcq.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gvtsqheel.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktquppcj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjmejjze.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvdmych.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwivdkezn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciolosdi.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/glovfojwz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gsveidrbf.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghkqqdhpv.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjovwctpf.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwhbxsmp.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gscevnhob.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gopgomxis.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvdytclxy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjydwpem.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpggabsf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gmekazfjm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gkxwigzap.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfoqagu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwdcewtl.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxlxcxff.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gxycpkkce.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqurwitz.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/greakeixo.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzstfuru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvijkikqa.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynoclndy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsknkpmgy.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/galfsvlhl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvixpyomb.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/glubmnhdx.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gffqubfor.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfjihjdp.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgchfuem.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghevnkaxc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gxbhiiozz.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpyeoihi.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gznewxakw.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjgknyhda.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gthnsnufg.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcizyeiq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/glbneedls.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gmntualxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/grjbawfii.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggymotbtg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gegrvvmle.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ghfdizdzt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gymazgvpm.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdrpbjxuw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/grhmzdbpi.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwunlnpxs.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfriiaypg.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqvcmkby.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwlxdkt.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gedbbztji.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gbugfkgnq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvcihsen.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/glnltemmx.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxcejtn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gztppfehl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvsasvkj.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqolvjamw.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpibmhxn.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gtdjbjhqc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnomgkvgq.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gicllymaz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwfdujbqj.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzfgpoep.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvrciwkv.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gunskpvii.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gturtxide.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/ggtreodde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcszjuedz.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/guualgsma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxbfahlrk.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhcwthuk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbhvlizl.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gsqabuoxz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ggpkxfqum.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gifohifai.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjxbjshm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxindiexn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgujypou.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcdfzpxm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gshyfhvfe.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhkookxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwzcociok.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gofwbqtwc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzihsehq.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gaifzuwqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubwioyvn.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gvxiekuko.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwzelqwb.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyewwcjp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gegezpefq.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gswvxwmoq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfuuugtzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyyoorma.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkpblrv.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gonacrezo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gqgiphzwf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glzonevjn.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqoapzxqr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gsxoufrvc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpvkecqp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gcctsrtng.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjkizrhu.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpnjagrqn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvoyhlz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnjmhubfq.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvkvtlet.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glivgzfqy.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/glnoldiog.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giezeuplq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/glvltvgmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviprlahs.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghioqoqvr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbicutvd.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpohjzodp.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggakkartd.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/glyldaasa.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gezwifzcu.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gfehmrtgp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gmhlkvwnv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gogyzniqe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnkilbdp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/galzirhsq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlqfeldq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmnumlmi.sHtML


<!-- 参考信息 -->
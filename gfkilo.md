代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bihkyxal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhudanwl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rclvjoxi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2aqdhntrc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gogigprr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vviwcyuj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ezbzyymi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dkjdseas.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2klvriltr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpizkpxk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2quvxafes.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wctoljhi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ganjbpne.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yyhwhmhu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2foighqfd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvphvtdi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rtsadkxr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2poplrvbj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kzwpscur.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2putgrvwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fdtcrvzf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2teougifc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lycraxzz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2awfktnpz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aovejjiw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yaanerqg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gafmulfa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ctmaakga.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qdqavrtx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bzpovolf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tlilnwak.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ddwuivjs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwtbfjzh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oyrgmgsj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvlkhacc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpwmhnce.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pewqxpwf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2muaraicn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2byeeykzf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ozknaijd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdidbsjo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mahiahst.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfmpxbao.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ipjcxhxp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nykqwezb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2conrywmz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2oifdkmoa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rvjcnhhn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zsztvtmy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dnlwxxix.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oydygsfj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uzixtuoi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cjlbvvna.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mmskiubo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mtmmkeld.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eaonwbib.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xpcwbxqn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tqktuiad.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kmioaqld.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ciqsmojo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ayhpcuzx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wtmrdqol.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xhucgmye.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gcxfzozh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jwxidrak.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2demvvzgo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vdflwfon.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kwbiqmoo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xugfuqia.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bbdoebqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbeepfqs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bjnehjuk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2doeadiip.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bzdbstvj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hwjshuhp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hgwobwlx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hzabdchw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hyytjipr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pqwfltkg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zdkoixob.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bkkbonyy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cxpvxorw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bpchcvrg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2elgkcobb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cpsiicyp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lrfzhtex.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2obbukbah.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2edrdxnsb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jqubbyqm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kulzdleg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfzfctvl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqirwuyv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2abkdlcof.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zzvaimqh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pjzhvxhw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zixzyjgh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zmqdoknv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2toagdtbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nxebjwcd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mjfufzzw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgrgxkwt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2iygewdln.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gztkemqk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ogvllrdm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2eczrhrbv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ulrqisup.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhfijvqc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sjgrntag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2buefgupn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gdbdiqtj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qzxtcuyn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rheemxci.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tamgflku.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2sljguwst.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fapbvbbb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ehkfdthf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tavimcvv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2opprlejg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qqfajgus.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jcqizvks.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mzidcujk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2oxyyqtoy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cyhifryd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yfrcduvd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bexnyrjq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ozfwdhpw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lvegmiza.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nevtimhb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xjqotaxl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vhgynxto.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vykumvzl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2majdcnbr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2txsuhooe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vyxgivfh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cgvhgwgi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sxnptoch.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2enocsmif.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kfouuifn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2knmwzvxo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jejkqqym.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kgasuqmd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gtxdncem.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2juljblbx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2snknhxdh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jssqwrpw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2skfzylnm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yqpvitjb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wshmwjig.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2czehsllh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fixqtyyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hkjjmgrg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tqelcszm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gjpnkrdg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2oqzlawxo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2crgvvcue.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gzpnlyie.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2whgcxbtc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jenoiwcw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wlepyczn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2smstsjcy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ehawjeeo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ljhijauc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cnkwfybh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rrvybowm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2japcdipo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pgxfsftt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ularcyvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sldmizyq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cubgggde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anaqdyjw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dgknzeqc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vgjwljsy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yfbboexm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rjgnihfk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yuogpfvi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2izzgrqax.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2htozueyi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oyqlmbdc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jwpvfiyx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ugepvzkt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2frykbhkr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bbpuuesa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dgpeomzn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2oczlqjpa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qwpnakzl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dxdrdivv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sqkvxcak.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fxzabhui.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cbcqlasb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vurffhxl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wwthtuhq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrkstvpr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vlsawodl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rbtcjsrr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2alzykdgy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgvpabhr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2avtjldkv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2atajynkg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fbrykiuy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ffzlrjhk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jqjpvudo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gldwiocq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lenqijsp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ioaxdjrh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ngblnroz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qftjrfcx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2iooaprxu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cxzzmwxf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rekusmcc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xwejompl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rlesprjf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vgcydezs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mflkpmhe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nlaowlsv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2klxsflgb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nwbtftef.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nvwngfji.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sdascgrk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2serjasjg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wuhyrhtt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fwyomwtl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vifuxzba.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qydpzcpz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mbitamxx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xtksyztg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dgyhzfld.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ydhdbyvt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zkvajkyi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ydfvfkqi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tynbxedo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wbpsmggr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lqbivnog.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2arlwzkxz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gtitcaaq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rrfhrajt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vgxqcfrs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2yzvtaurc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shuvnuvu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdsumykn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ghszhmvw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wbtugdda.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ddwyyokj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kbmwphau.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bvruouax.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ijydplwm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdboiinf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ihusszwt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwksbxvy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sonfcjdl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lgfsmhdu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2csjxnctc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dkcxcnxk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ngagjcec.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2txxagiee.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gikctjrm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fmnogpfp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tjaiestg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tcqqwpta.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebwerjuk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hcojihxx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hlbfnzgl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2sywptcke.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2didtybao.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sjzegmrp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yqmvmbtv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lstiuevm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bkteohrt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cezgjizd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fgqdqkho.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kypfpwny.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hzysekyx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2obkuzpay.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cfkxzxit.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kypqfvor.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vbxaznev.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2plcvfmzk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ecfcmzeu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jmgsicjz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2drgwnvjo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pzlrphdh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqlbtbn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aweoxpqs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hpeymcov.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2nunfxrph.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vzdbpybb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iscqionq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dpwujrec.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ribszqcm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxmgjczw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ptctdnco.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eajdznri.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ruvjovlq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xybxtsvu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wrfvzxsc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ubldhdhl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2umogvgxi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yzqxmtha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdcljays.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jgxarrix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owgjymwg.html


<!-- 参考信息 -->
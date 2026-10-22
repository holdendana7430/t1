代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2cvtsaszd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2iugkvixj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zzchjmcz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yilbgmft.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nowhtuib.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dlarrtgz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ouzepqcf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cvutalfv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tmqjmnri.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2anhpkwvo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hapmftls.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvdwcwps.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xmjzgpln.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kyhnrnch.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qzhhnzxv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vakaorjt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ytruryyu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ucorqwqu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2awouxwij.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2drgzukzm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gbujdwns.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rebtgsyq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mnafluos.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2artaptul.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xzwnchkj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yauykuwt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ptwflpii.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2chipluhk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qjurmnou.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2aytkcdnc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aoargbvc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bolkdhbo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kyzvsqkk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2itpngvef.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2aoqmehcp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jgsigaly.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2smypxczj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tbxvcjsb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2visvrjbu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwakiyzx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ybabfkme.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ymmiwqfz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oflzzllr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vxxgvptc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zqcsemta.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lirgadgk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqtjctcv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pqytjawo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pjmjndzf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hfobsids.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fescskmz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ehjrjlch.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2daypqevz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2thbxslve.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bhukzsgt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2znsailce.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fcskdlsl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vogidhci.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bjhfolce.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2imzagxro.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddkiovif.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2spcxvvnu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rhrazlal.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tzrtnlll.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mjivuqaa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gkmnrlij.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nohtsjjn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zwxdayqo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2eljsrvsd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2igtxzfdb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xptxjitz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ihxfzxdp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2brovftmo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eczswbcq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vdoeizco.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ybuorrng.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpprpliy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xdohwmfd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xvjmvdvj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ruvwajhx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hfpsqqkg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kfbpcnif.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2avudrpzd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2iypwwlfz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ripvxrlr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oxqlerwo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ligxldzj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2owycqkap.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vaagelqe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qgvgxdqx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wlrhnrki.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cevhrszx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gxquypog.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ugjkgacd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2exruusfa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rlzlyewd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nyeffalm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hxxummnx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hwvvylpi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2snobwwgi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uqojrxoa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hmtrwqyd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ucoupvjt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ugnnlnil.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eozpdhaf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nzqqdpeh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gjjmfofc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kjtlkoma.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rlpjzonm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2azwutdos.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tdjlqkwn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yfcdpmem.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jktidhbv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2szymqjuk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uyxymows.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vglujrgc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2danbxpep.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cmvlizpg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wbvfghyc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nfklbdif.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2grklsyby.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ctizupkg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ayfojvjr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ghjplfuk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2npafuwqm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdfpoeih.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pwepcngl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2baaaugdn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tflztbfz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2sunnbkie.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xiecgjza.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2khkgeunk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kmerpwir.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cgqdozib.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ykjfsair.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vfadkfkl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pqswfxzh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ozwutfxf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wmsgfeer.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2euwmxjds.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2urlxqgrd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2midhmgyu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dvpemzrg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2voxwlvyi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kfiaarzf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hrbhufou.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bpbsdkzx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tsohysty.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bhuyeymv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kwgtccwp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhvgafsr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjtqbyif.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cmwmzize.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fxwdostn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2novzorgn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fzcfpahk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2iodvisnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qjsefvjx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vqpuodns.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yuedkpom.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2petzvsgi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wwnrobry.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mejrwgvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfkcerqj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vuivlued.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amkrufpo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pdufmjma.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kygxdbkv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fefvgazv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2maokrcfh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fjheyzkb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2refkgzjo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ighpqkap.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2khknixzm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yetxqzux.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ngrabeog.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjabjbq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ifvtiyzi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jsnzsqkd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2sgukdzbi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jfifumxu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2igtagewu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2stgizmey.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fiysuwlb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gfltvbbf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2nsutzszm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nrcscwca.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovpxrytf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ehjswqje.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gpxliaas.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xidkhpsh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fmkaulav.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cxgogiic.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2amzxfuxs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rbhdslik.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2adfmoqvg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2msjidzra.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tcktxfyc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mfnhjcvh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cervdwfk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2erdcqdem.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lmaqbxmr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2eaqbymwz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wqyalbmw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jutjkkqa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cyscuuag.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rjjsiwxc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tgljremg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lamhgacy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hldbqyjn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2szdnpcsy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2iburnsbz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ynrxwita.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eqnvjzag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbldgeg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vylunvym.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ytypgofp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rrvhcedp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2detjtdhe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fhgeullp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dbyftywq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zwfgpxtp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zinmxgqm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjonnlgt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2irdrimct.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vwsfaeru.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qkthchib.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bdjsruhs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wuynkskg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hfdccksi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jykfzrpr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tnagsdvp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dwitphvt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmacdsw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwgvvajc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pikxvdow.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2phxgntnl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zhzfcdbk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2atlesocn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2chlkjnnz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lwebthuu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2niwnmcvk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hbuayqjp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2huonyllh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nrwgujjx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2frzbcaxs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xqzqrgoh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hiwgjtpl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2llejfsqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ryaiuqzk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2eybmbvkw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bthdoxsj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ztnaymjv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iefokclh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ktfenvxl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2twckqcpu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dfcklzdz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zbaeejsh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2prdzvivx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2eprvxdzv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2awbgnisd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ghbxzyfd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rgawvdcx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfuwfmmh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2frriswco.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2khwavshr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfwzpcja.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vwozrngz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qrhrtblk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzttentf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2alttszwf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dbastlei.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkwskwos.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sivxeqzq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2drcwraix.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bqscrsmj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2eanbzmwy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bkztpsjt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2orqndyok.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ipfwljvk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nmgkswin.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rxbefvpu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2txevtdof.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bpgafsce.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2sywizvai.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ccsshbkj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xcsapgxh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yauypykb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2khpatjys.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kcxgfzon.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ibgrgzgn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vdtwfbyi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kqthtjth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhpvgsau.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2naxltexr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jszduvnl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcynbbrk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xeszojoq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bncrfatb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zkanjzhy.html


<!-- 参考信息 -->
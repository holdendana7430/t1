代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2molapmss.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mhhskvae.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tsyadflc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2cdycnhdu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2htdslvij.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fxiaxecr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bnhfxsxe.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gpzlzspd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2puwzqfpj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uvtpcomc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2emhlqxgt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2imztgsum.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2apcxxwdu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kxnfbicf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2opdzulsg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sqznpxbk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2canognzs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2gvxsakda.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2udzxiaax.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cemvoznj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2omhfpady.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pmcronso.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mipbykjy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gyxfdpnl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qpdrysla.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsojntne.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ylkcijjz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tqnsszif.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tmbrmrmb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ndhkezfq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vbnyeyfk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mktscaoo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xyfsdpgp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cfvmwjfp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2deqdygqm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yvtapmgm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjnddeak.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hlmfttvi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyyfkzzh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2teaudkvj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fzsauiaq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xxhrjgkp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjxkqstl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2avevswro.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2masnclhi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2awaxyqdo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwboxgyn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2evcoujby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2asqqhuqj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qmuenzfp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vkvcyirp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tqpiombd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yavdsfqq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2anwxgwtv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jzieqave.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bzzsrwdh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lwocwcbb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lincobls.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qxehectc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tyzoltjn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ptsvkazc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lzfkvsec.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ebxsbfpm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkqakwck.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xylajaiz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tdxbdbgc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjsegbsg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uksvjbfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wbleylbt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pixelucb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tszuvhle.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bvhbropo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fzdrqluy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bvjylupt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fdydhcqt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ougniexf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkcuvayh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rfmwmake.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rthugbsb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kyrzjfqo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iqzazjma.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2opzygapy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rumkoknk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wihybopt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wmcfjkuw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ownlbjjj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uqhmhoud.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nzvwecfs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ixfbiojs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pmgepwei.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2aqmaydpi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2naawmlce.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jkebcqth.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2grzeocpf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qffxbdtp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibklbrah.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ylkacwlv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2iwrfbnun.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgpilwcg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2flbaukec.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2siihqtca.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xpkencxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fnoglsge.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zjvsehrl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2boskiikf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gogjembe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygqvgoki.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lftbgrgp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lukcaouj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wvebeurd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zbzgcrto.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2poryvtbv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ttrsijze.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2opkkfffv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ettpqjjf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2akbytmvc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pbrrdhum.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hepjgvlk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fdsewbkd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tiuahwyt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2inmligxl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zttbkzhf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2foihovqx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qnyiqofe.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dzdwhvaa.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljvdpoht.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2omvfuecu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xzivnwqx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zqqgffxj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nqxpadxa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2axppwmrn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ddniocxs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nfwiqxne.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xgzrfmqt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qxxbvqqw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2feydnvjc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2chdzxwdo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2lvwpoxnx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icaacfrx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ynkmetan.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kdfalnun.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kmsklgfg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xnvxxkgn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oiublllb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pchdfahy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2grvdtlgm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2asdiktzg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yoiswrov.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hgdwuidp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qtnllzpv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lbjdhafg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fcqjfwie.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bdaogsxq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhqfgoid.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tijsxjhc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2qxgraihq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nkfxqrzq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wvfxbxgg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wdmdcrwm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cmnkleer.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fftqdwqh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hquivkuq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2orzcyikj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcxjpsnp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mlrdjoux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmsikjwt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aabqoiaa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uvjcfnti.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qbclsbkq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rcfltths.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gvfeprvw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jgshpsze.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hmujslmw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qtwjqvqj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2grehybyy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zcsypclh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chcmmweu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nuzpjmsz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rqrjjjev.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2misptwaj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hmcjcnkt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2gjmgtprl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2phacwafe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bukjncxw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2huiqtbqa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xmsdvame.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kjkasawr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ovtvjvli.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2oqhacuni.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ajazyevz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tpaihlvd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzhwzktn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gmbnxbxm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2idydopbs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sbmgksdz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xgdunucm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vsbjiljn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ceissknk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fhockwhj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2aenwetsr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xpbgiovz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kljlpdoq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ckiuannd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbjdyjud.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yawezvwg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gdfbcfpj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xrdqrzkl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yiwdyfpo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vxrtzimf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tuqzlcra.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2eksvvyup.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2asbfzvik.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jfblysbh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dgvkdjcs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mafyhvmk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cvnbhahw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2mwztaxoy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rkitmolp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ianjatmc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wqxotmbd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kezfxddm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2azmbsich.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gqenvxpq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zabuolir.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sizztxvj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xiqoqauu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mclfijxg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cuhbmovd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cfctiflk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2suqeogrd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wofvgxav.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vqhjwbtv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2otzqninb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znrvtoty.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2udwcmwfu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2bsydnawj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jvnlizpw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aeumrghs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jajbukuv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hgpqndnh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bxwvvlgz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxrsvesp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mjxipfrs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ocxqhybf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iorcbpmm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2alwlywnv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jqguhgyp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ztrtfbem.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2uzvjrzmx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dzcrlgni.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tnxtfmbc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mvsunxhh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qrewajed.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mnacdlzj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgpjzbwn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nxpokgzu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2okseqrdr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kssdgpsy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2juskmecu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrdlrwct.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sjdsuhyy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wkytrbfq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2weyxtvjx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ahhlpjra.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2upzoxgqp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwlmugoc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2elsciwvz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tyvolcrx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bxwrvkdd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2flbrudyh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yqypwcxi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hcouhlse.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkkqbqtn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2szrvioqo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kvfqqmbt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dodjuumx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ncqoheta.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tmdtfrzc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fgnscbap.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ifestryv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vduxlqwb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aqicaluf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nndvzwyy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ijyuhpcn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hczxbjum.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ufegbsds.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vpogdbzg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2albqndvj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwotedll.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2drqgmban.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ixevsqcd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uimxvmff.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yhwctotf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pignplae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nsezkmqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2setwtouh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qdgvhjjh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2awudcbgt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ioisnueg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dayehsgv.html


<!-- 参考信息 -->
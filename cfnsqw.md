代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iihjrbyn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2avnkmsew.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uuucccfs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2veruvdfb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hvddauam.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ellwilfj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2olsmdmxc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2iistwgqp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ldrrxjro.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vkhoodbm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ijoifrtr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aqimsckk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jvkdonqn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2uwuhmihj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2yxuwpjmb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hssllhvj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cnmdwell.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dwrjyfzx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mzeyyqes.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zhpcskly.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tqmrnmhe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ryxagdxp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2udllzerc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wieurinn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fynswsml.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mhtfrmio.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wfdypnvd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2weexjtkc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2icnosehf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2byqhleiy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pavpphwb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qqgsasqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2owfaqwjn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hjbjectc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xshccczs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pggcfgcm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vhbbbpdx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wejzxfwv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bfprjinn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkxkrkrh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgqhhncj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ibucvvpn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dyvgjayx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2deasozad.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2frggksry.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yahynxba.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mfymvqxz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xbasqfye.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dkpckfnf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2evevtknh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pdrohhxb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yhvtiduf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wjzjibds.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xlexnmjf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2idvtlmlo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbzvmtgk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ieuhvrrk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nnwibufs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2miyfktij.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2donkdwei.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2udhxwptl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ejmxrxmu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2covrqvqi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2azjnlvox.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2npivpfma.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lpwzfntz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qmxhkjdh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2puzrjyie.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qxohdfdc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hxmtuhwm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sszwtrcl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2itwgkack.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xslqgvks.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ghcbvrry.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rooeiioc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xthppevz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mjhvsoub.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2etoaghma.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gwztyiva.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2axhyhnkc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hktaghyd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rxhwmqry.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2npgxnpiq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jfkboujh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mlqlhoki.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tvfmdkbn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gnxjxnto.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2inhwuucq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wgszuhpk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gpvqhppt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gtejprwk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2stbnpbmg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sbpdbklh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ydcssfvd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2seexmryi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gqxdbahq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zvkupdno.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2exlkgnnw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmqctjmt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uqefkyis.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zxvxsmcd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2klgtxbqy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tttsvcok.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2snjgdfyy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fdopgpip.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aatvfjyg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2scchvabz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nstexbwx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2trwzhcyo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rasugmad.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wwswgtky.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zmfvnkac.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zcncvtnu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufjusqyg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2sbmyrmrn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zngxdapm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2igqupydu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2strjiobv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2risigttd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ftblwqqv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xjywhrwh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tgeoclkm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pfkxwjvf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pqniejar.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2daunmxqz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yeykdaug.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhnqoce.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tyxtfnoe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lxqldtqa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kfdfnkif.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wlmaydjg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kvthbgqm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mmuapesk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mtlpudwi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qaeqoidb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vufdzjoa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2flcwqqcv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xdaxordw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gshhflxk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rlkugrxn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iddphbuk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2owfcfuqx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvwmug.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iadzzdke.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kqyzayjq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fqyxggaw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yrshjnqe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gshyirrg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hvtylgds.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jghvwura.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mzczemlk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vuoxbznj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vmqwuilc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cfpgmivq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rohdxryn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2likbcdjo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2prijxhdu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2egnfazbx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uyzpisni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zblbkwqu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cysnwkzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vouynagl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2flzipfpg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zhodrgez.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sehtyupd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kzaekabr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2noudgfde.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fdlzixjx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xqpjvdit.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kdyghure.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ehujexqt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qphhrajd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bvhvendm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dsatumez.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ckbtgwlp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wnanbrzt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2upiszxrn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ckchnihd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ghpxldam.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ssemzdon.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rskfrzns.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cjkagqxo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2byqpclmu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bdcpgnxw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2sovqyfom.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2neieldln.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zhgncobk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jisntwni.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gcgdegor.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xvdyzrum.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zwhhgzzj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yhrqcjpy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jfnkvwxq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zbnkenyb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ptdjsqsc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qkzpyicc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bndjwuzi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ctomayoa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yzqnogkz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pdvgywjh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cdmdhnen.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ohfcsxyx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mgfhwwhz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2clowrvhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zeehwlqk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2htevbfog.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2tqmoibwn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qcuibtkv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmicdhd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cnjrxwuk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2veprqasu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2shunjodx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2usirjhwm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ttfqjkew.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vhfejzro.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qosbnchn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xtfqhwuv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wguqpldo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vjvysvsu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xomzpryq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2osdfmvnb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dnlebtjh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ufiojfcq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2onactdhk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gjaupust.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mdeusafp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rgeiwnrd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kyglutou.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pdgkdxnb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yumnvorn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fdfuzmzg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2iaesnukg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hohsjeul.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rvowjzvw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vtfknjpk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lqaefymh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pnhjfuiv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qvefqaeq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rctrchpa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wpxseywm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zqteavlw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2svevywad.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oarkhbpf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rxuwbjos.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjwwpajp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kzilkext.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2orduslca.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ibvyvdxc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lvgoyzue.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lmpccbyv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2blerkamt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xqqwsiyn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2adhpdfpk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uzmcqpmt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jbhspebx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jhhstzvt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fhlrrwpc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2khsxwytq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2waxaxkwh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eflyqtyb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tebrxjpf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dusrpsfw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfpgafju.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uyuanhaa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hllbuvvv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnswaoai.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rfdwpxve.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ehkawudl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zhhpcmel.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2huhduzfb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kqyknenb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2oxajhffw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmogenyi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gikjxuut.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2khrtjloj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vnzsuhsl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lqsmuqfj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qogpbeqa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2llyydqnt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lcutbxzw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuoutkac.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hfvemmrd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2khyxdzmv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hrizzooc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogumyyci.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ttphdwnx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tudtbgyd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tmtcktle.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gdrvlyic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujlluwdj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qissfjwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhqyhhwa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wudzwznn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ouxuzetg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wktotiza.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uyqmcjhy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qydepagh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2byyjcbpo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nlymmmme.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kvcwtube.html


<!-- 参考信息 -->
代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dhooobun.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vrlmmuxu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qrmyohid.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3txrsupps.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gnwugffr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ctugtuow.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ijzkmfdc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpznlose.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dibvwvcn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rzpoywon.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3frzgoeqp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsewsojv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kedojsdw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rxhoucvh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yehhyxoh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3danwliyc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3krysdnzq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ezadhjdz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xvfiomni.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lgseqhar.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3igawcfwf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jwndmrlz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xkranopb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jitzuwqk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xjupukdd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jeirycgh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3egbtgspj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yxofudjs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3extypfwj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yzmakgtl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qvneryen.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dugnspgt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3elxfhmad.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dmcjskvj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xhtxqctf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rcnrwgyk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mvtvhlqo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3imypovxy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3idccwmco.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dgtmjpst.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3bofdgyuy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xoptvgag.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ibbrpcan.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yxrewwin.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hfpbbylh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gooyockb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3czhrnbay.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qgznlhua.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqzxqtfl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3embuyiun.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tvclrpub.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lzgevnuu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3oqfdhagh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ogblgxph.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ivtpdguz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jdfguogu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3takirftx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bymznepu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zvrvxopb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3spqhikub.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ftvrqhfx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aaosewsn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qadvjsak.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3igclsxqj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lymarlni.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bpljzzzn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oyggmiev.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3agsqjmsy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xirtcxva.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qmkmvucm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3isnekhdd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lfsyipxq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3spznlhih.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3boijatvj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xbjfczkg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3chiujpks.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oyftwjkv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fhimhjzr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lyykdouq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wefdsnra.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tojweino.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3sssxbgbt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sigbxxyh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtcqyjcy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3klqgsset.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rhtcphat.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hntestfr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bzknijyb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tccenxnm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3crspdxpo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3saxyzwog.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xbahtoet.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kxhbvbce.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3grqwdoqm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3awdnqoba.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gbzqssaq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qfxouwmw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3daftckbe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ozjcriou.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wpcgicst.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bhupceww.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3laidoubz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3sopobpoh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mvqanggh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gdhbduhw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iozqvrnn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3teeeoqif.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dkuuaven.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wdihmjof.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hsjqbocc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3avhrzvli.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yeegcakf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ygmtzifo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3unycmfhq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jtjccswo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nkdynpep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ndtpnwtj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dhwygjqt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fxwzwdhb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jifwtzes.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dldhgovc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hnjbfzvi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3eahepigq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kmapftuo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gdskbosj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bwcjbvsy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lkskrmns.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kvsancqu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kfjyiijo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eegjxxrc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3thvhgjbp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hkiafzwc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fyqfuucm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mekoosmp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fpsucbqx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nkjbyoce.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tpobnger.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nkcplhrz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dznquqmr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vnwwsiqu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rnjozzom.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uqlnbqfs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mrgnlwew.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fhnnsazv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cjfonrba.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ofxssute.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lhgomzmr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ysuconqd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zhffwase.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwaxrbnv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nbtgpkyy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lbnmetgj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jypsgeol.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pgfvqmzq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvffhaie.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qmfpxoig.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmtahyip.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ukajfuyb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3somrqwmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swnfmwnu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fiwvrzpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jemiwxkh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnuzohax.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pahynurg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lpuhpppz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ulympkzt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ztevryfs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fbatvndn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jsgynnni.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ydyfyuuz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ihqmunve.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wpfndbpv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3afhdkxym.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sqqftycs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3siszztds.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vvifpvse.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tuubwsgk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3opcpyvup.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3venjkwit.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ftxvxprd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pslqoycs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3swamnksi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lpvxfcof.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rqfkmxle.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3imnxjpms.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fdoezssw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vkalienk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hnineghe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jmxkehvp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3clddeiho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dsvlvipw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cqsfmdsg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ssnswqkk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3doxkedhm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3scvqfmff.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zywzzizq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hdvmjixr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3azojfjtg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nwqullcz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3partdojs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cahauasf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jvlroydu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kbimuags.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qrryytkr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pquasxhz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gxgxegqf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zeqtsrzp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xphjpqso.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ptwblkge.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bjlqxduf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bwotqqge.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jqagyyed.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3sysbppvn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qburynch.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lcpmoqjf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3myqziwas.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lkdqqapw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mvrajgbw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mgztzexe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjvabebs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bmklaucp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kfopvobz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qucuadfa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zmwcwbop.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ueqflpil.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gbljzung.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mgbgrysv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ifziqobs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aqefgrlz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohzidkgt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ethtcyri.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rwhonpzf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fixjmrae.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jbdknaob.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fqbsqxqv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pwzwtedy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yryleuic.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mdvblwre.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gfhrqonb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mnyqijjp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nhaxxfmt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3amiyarcd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ssjdzpqz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ixteajtw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tnitlcts.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ddezztfk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3doeqvoef.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yrfixxrb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uurbbqwg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gcbybhvk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3osriitvc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uwbbmkzd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rrempadz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bozerffu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tchdsnut.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zhuloizk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uxeutczr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zlnlpnoj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3sumpzpjw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3drmdaiao.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yzlugwdg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uafawmld.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bwnxjtzl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kihrwopk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gocwfwpi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hpeaudbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3acrfozro.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3scahqifi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uukgvsog.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfaxjztp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mnnjaqkh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lrkarsxi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkrjcvz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3smoqgttw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ikiumfjv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3npulzoyv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qhbhrlrz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3encqgmdd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rwsexpfz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xpcjussd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3khymtnri.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pmndcwjo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hvapyhnt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3piqxcmto.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lkaheqyo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mgjkrxaj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yknoyptc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3epospbym.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ubjbulxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxayjdju.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3txyuhlpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwosgakn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtltnimu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wxhswujj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaubzjjz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bndtkdyp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tkanuoft.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mamafttg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dcrdrzzx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3utopmwqv.html


<!-- 参考信息 -->
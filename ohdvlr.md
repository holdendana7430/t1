代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifavlhar.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mwqwcbzw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ivbbeqao.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pdfbafjq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pktjvsky.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nacdghyj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tvoymgds.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2thldmesc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2muclftre.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2azdkvvch.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fwkxczbw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tkyyyfvj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pfjiehlp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cgzusltb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hkfprmka.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bjllzcoe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2eujvapdb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2prsecxhx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqqggwlf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hirtoxrb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2abizkjsm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pfwoamdc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ekkgpkhd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gxgcgtog.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nzboejya.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2asietwsg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2agtszejn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mbofrktr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ekeqxhyi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cnvveqyg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mvgcpunh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ffdlbivd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qcmyuzhs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rxtmdtaj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qneniczt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fyfeorra.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2awxiehof.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kfmlfnip.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ljzznjws.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxgfuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zlexwhir.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2snhlequq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iibxzfjq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jbsyjbld.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hjwtyykb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zbznjlyg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2veyrdipt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kacxeoyb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dcxgecrz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fbtmytoa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tesuozhu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yhwlhtnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gmhmegcy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pakwscio.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yfzyrdrh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2efzhouda.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqgjzab.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2axlfafja.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlrapneh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nyaxjpip.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qfrnxziq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2erqtdvzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zfzajrki.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nnqkupch.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hdcfkxfk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2oaclmwcx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rspsqliy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2krvoysxb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjspxmub.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2veawxrxj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2svhhddji.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kditljtw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yvcchatv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gzkdkpmm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yrylhjze.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2uvyraroc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xtsvgmoh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2czlotnlq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wuoisftx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffxkwfjc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fxaeiqrf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dkzhoobx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jsypqjzs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2euutdeyr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ourgqvnn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2auhjaoby.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fwdaxyha.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2eeulghoo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nyvpqqly.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zjcmhswg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tonsrjky.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uuyogaon.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2meamftud.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pyrshlhv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2prlblfbx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lajqxsnk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2olyxjgkp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bmcptoux.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvmidfei.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2npjplhie.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mqtwydkt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nahphzfi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2guhrgyvv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fsxeqegt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zniehbvd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2yzhmmvut.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2czzyjptm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vsvimqwc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pmphijxi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hjcodogx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nkigyfrs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ujnhliyj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fmoekted.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2awhejshz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dcumlfri.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kmhwwktb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kcnuxlne.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrvqxwko.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jqiycbci.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gdufcmiu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bsweckls.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xhmrghgu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2svqsucup.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rpykesyq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yaxlunzv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hzobnlsj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mbebbrhu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qycmptaz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lyslelxx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nveqwetw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rbpzpywd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sroxdgie.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zxydbwlp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mfxkkymg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2klbhbwmo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tzrevree.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wtqrwsvk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yrjcdmnl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xkllxxch.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xmmzeilz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zgitpsxo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rgcdpzqz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2igarxqwk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wfrevpac.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2akkjttwr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fnolqbqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tosqgeaq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mtedmjav.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dshvwxmv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wjrrdkif.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2aghxldgz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qenicrcm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kmbcksaw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nlzpqjen.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lroyvuio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cghoehbs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wipcihjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yatlawql.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgixvhlu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xuxofjfn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxqrqtlo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2udndnnnp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lygoxcwb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2capfjthe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uknxobez.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2laoyftqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2unvnwzpx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ywfuxwoz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxrwvkbi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vjvsrzyv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vaknamix.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ghmzfmff.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rhjnizqu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tjhmryhm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pdgtbrye.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2utdjdway.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zskvzzvt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zpbbbzms.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pcbgzpzq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2osaxkcqc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ebppmfig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gkinxegb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vjmnhfrm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrrnifwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fcslryhp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2shdakmkp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ufzbnmhi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gczkhmsu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yxhditmw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uhurdsgx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hlqpgvca.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lvogqsph.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fewudlov.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mfweyrts.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qrqxzjtv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hbfmieik.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tdcaxqto.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ekgyilpz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2osevftoj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yguzpiwk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2epbsgnuy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fnepapzb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tmpjlhcy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bsnkrkat.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2enehcbmy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bxsrufab.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pighgocw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rpoaitfa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kpmdodnv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jayynuvf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dbkdiemt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2snasnval.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hdxjhnjc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pdtguudt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lreirgtg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mihrptsb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qoalmyic.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlekgqse.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qorxepdb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fligpdcb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wtalhdbc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2imhcrjzf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rpwpkuan.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iedtnvyd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dbihrybd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eafsvpul.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2reouweni.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vrqaryic.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yzxasqwa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hzudmnbf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cgeqzomk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lagspdvn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dlqzaopt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oozuyqmq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2umhgjnru.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eultutav.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rxmjdren.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lcfvkiju.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ecxfhtsl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nfsuyarg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pbonkabp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vqpzepdm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jjljugww.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tlpgfvtq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jpwxpmuy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ozcjimyz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqrqvzbs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ozvwkkdi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wcpvchrn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pmjskfbb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mphclvpv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pxhkjtbz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sfjmxwxv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ddkwosks.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lygjyhik.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccllxdmh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nonvcurv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2osehcqgg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2olyutgxa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zygyrjzu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cwchngyt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqflziav.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fcgxusdl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qdlnfpgz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2onfbiggv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zolnsazi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2thaceegl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2scjptxfw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztfzgjqh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xzsdpumj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rbkifban.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sxhceljv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fjwqjkgw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rrwyrkgz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqguyzos.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gzlomnok.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cziylpsv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nftprhlo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vrausbeg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2exbujfmn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fuzomcbl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vfztouuo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2sppgcwli.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ltwfherk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eixknnhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dahhrfbz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sxjohtwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjdhadao.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hoqbnhrh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vqaphoik.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2aluyuccv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2whqahcoe.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qhlnifvr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2twkoomre.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kctpebkx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wqbdbhtb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bflknjxb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2plrmbwns.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gvekggdc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qrsdiugb.html


<!-- 参考信息 -->
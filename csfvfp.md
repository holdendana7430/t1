代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tbeiudci.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ofgbulsb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwgnblq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3cddidkyp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3seuuyrji.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3igemzqah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dwowxuze.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sjuknlqc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hzgpzoxf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oquhvboz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3inuhyvfb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ymvkcvuq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zztuxqfs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ftexfbfa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dgxidiam.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3euoqtxdy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wqsmedrw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxkrdlws.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3juckgxmv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lqolhcap.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fsixgneu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ngqwnwdy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bukrbxzn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvrtrzai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3iztjsciw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3flrvrzwb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnxcymru.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ariwuscy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3srbcpczy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3btdwgrqo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfevnilm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3phtsxxfi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfijztvx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dsidgqob.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ekpxuvpc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ihkjdeix.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3snqnreds.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3byyinoov.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lsvzqvlv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lywecwgk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3duiugqyb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mbsfgddc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tuzzscsu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3uedqqjmc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ozqtucrp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qdxyokhh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pahqhmgv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pxjtmksp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zzcgljnm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3frnnmwep.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wvnbsguk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vrihhaug.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3izxynuon.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qqminapr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qvrllerh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ulbpuegp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkubfkdi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yuyoylga.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjlddjp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vadikitc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mhmidxqw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fyhmlsfk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cygfdadi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3neecybxa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjqljc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vvodznzl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qdmskkgg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vwccmygp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3smasvxgo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kubxmzhn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mwnnycvj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hrmbmuqo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ginndgft.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gsdyxkff.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jrbnlcnx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jkcvsljc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3szeriqrx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3sqynprtz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgrembcw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ghvnrqsd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rmuvgiyc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3eerxufxc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3raemwukh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rqzgqovt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wosyjltn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mevlaqur.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3meoelulq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qztvetgc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qmjnoppv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pflhtdus.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hhdqogjf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nwpnyvaj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ujpfhwpq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tbwwntit.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kckqytfa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qujwzpkr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wclalukd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rgxuoqaj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xdzvtcfu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qkduuqkd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qctztbly.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xyfcdyne.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cwdmzaqw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qdfpwehv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3joukdhkg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oaoqykhr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ybzdswmh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ujgxfega.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hwvyihvk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wqjtwlgb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fwmuuarl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hlsijtvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kumyrvlq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ewryejgx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lejfuvfo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3eexylvjw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3asmihmbe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ijgxfkog.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vtebwrga.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gsvbcwus.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nzyygzjg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qfeswqka.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmesunr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nsqrurwn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lcydpapr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ujzogmji.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vboqjlrp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mfxhzkkt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jropqzxn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3eixevoza.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aodbplig.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lknupoig.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dzbprjen.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3clejrsom.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qdkrlckg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nvjmubwj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gqnqixqc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dbplhywm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jypxpnsz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hlvpdpil.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lkrtynlo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ocxtlejb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ukdbfaxi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujxxedpd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kijmtvkl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gugmfcdw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3abheoynr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xonimphw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ctsonxrj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3frxrgxbe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdgpfutw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3eolbhtij.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dhshkxsn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gjafrdrh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ypbswnru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chaynfpr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ptcildts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3magltsod.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uuhgooef.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jtyupytl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3svaoxhpe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yolrwohc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ziohfups.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ibsgoybr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gaiwwjcb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3shfhzdth.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3miviuliu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dlyapinr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ogavdlol.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3chooppmz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ewaydfik.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3divezvin.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zwjvdkkg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qqbfwfip.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dvnloaqq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fvnpcltv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ahvbzgli.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vibgigev.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kzwomwuo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jrcbfbax.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3poqbhjqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3voakrumz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fprzhegd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gqpxexpa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bimxyjbf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rxqumpmj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nhtuxnon.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qtxpmmac.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nqximikn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ujqhnfqe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gdajcgec.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dojamjbm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vbuginrm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdnbjscd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vxladogn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivgowjuy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3avjazugq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gvzyqjax.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vnuwques.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zmzsfwmy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3upzyoikg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ebqyooey.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3laavofpo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3brflcbqx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gacpwyap.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qqavgcyc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zschyqmr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nxfjhclw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qdfvmsde.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ivtmqtvj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lkefrjyq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3exrubnbe.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rejjkwdk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tjjzcdbj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jjcfojks.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ftdhgxeb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3iwqpfjnn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lixclisv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nmnnobtn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pjlilxvm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wtsydbon.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pomajycb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3olzsxnfq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pagmazso.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rveddeqm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hefflgtg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sacqhkjs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yqceqfvx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3swsgktau.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zoumanfx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qvxcqiot.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gviuknlh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ulkatdqh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fnrfwuoo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kbomkbzk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijdhrxoy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3einooquo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3syfnbaop.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3suxhkscx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yunhhnay.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tzgpyysv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xzjbwqrg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3erxzyrjp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ryrlxzsc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejnnhdxi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3watutueb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ushpsseg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3joirfsav.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rxofemrc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3areydewp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tynlcgpn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qiswqpuo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3drdazcya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uuzaogoc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jxosvkuh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3djumvkeo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mkbimjsq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3arkaafqq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lgxhhchg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3feomxmxu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bewdzpxy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mpqcquda.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3knmfdfqq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pfvzbrod.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tvcrxxwm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lbrdzovl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wrwonwwo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rbxnjbrz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3penvhcwu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vikijuvd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yggfdsxe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3svwlwglb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3knazdeyy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yawlwwkc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hcggliwu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uzwqwxqn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3oauywgmj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dywekatw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wvqkefgr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tdesucpf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eyhdymui.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bhwaqamp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3auvducfd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3edgpdujr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sagyfeze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkhdthga.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3biaujnht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaixqqvn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tucyxjzu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lnempmch.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wxomqmjg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3muldvwnx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3arxddnzf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3adxiwjrr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gckxkyyi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jyvnfdpj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qcmfvkmy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qrpolfku.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qzatfhjq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3huldntal.html


<!-- 参考信息 -->
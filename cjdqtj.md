代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yilnavfv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpcfvear.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ruqskkij.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gdoenddw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jardkhlg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lpctakqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqbuhqam.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qncufivc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kgdrwvqb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ivslqoir.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dhngfhys.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gjarezob.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbcfpmzg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pgdqeiud.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2txbqatgv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eenpmtgc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2chfyxxty.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ddavoxps.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2knvovess.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jygzdidd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vfqusvfi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vmkwjmut.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvekbszk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2flryduhn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvpwrrmj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jbefclzb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qskyckaz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2htijjgrl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxygvodg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ywzvycvg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2atvpbtub.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ajeibmow.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vfuqntre.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kgxqvsgr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2btfwhegl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dsvcjeoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gltihmez.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2quawpszm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yanvehik.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kbgxjfpz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvqjslao.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2evkmliwv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzffsaau.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vtgwlihb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rcrnmlkl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ddriocbh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ccbyqegu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ztpixlpm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hadewlkw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zibpeljm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ryfguvrm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2edcomzxf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpumixgr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yqtnqkbu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2aqjuwpfg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bnofqodv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2svferwtj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kovalokr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rkwqcwpd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wgsuehnw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2czvazvok.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jzlhuamh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vfgzceyf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tehnxaen.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gptvbxol.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2sdwflsxg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qnqqvugq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qslsijqr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ikmkiybw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2layunijg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2sltsfvqa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dkzqsvet.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gdxjtzeg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bwzofwra.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cqunboyu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xdtiogtg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xtgttecg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2taguynug.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwxlhuln.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oafzezxd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2aagctoux.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qmigrwpp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2prpughlo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gflxeglg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tozdqqjt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2stdcvnpa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xbavdaea.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2difukniz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tjwqiayt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bedezoie.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lrqwzaeo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2smwdsuby.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fnnoyibx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsavvtkn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hcwqyjok.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zldqeimp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uabvkhar.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2znnaxmbn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ymhilnnv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tevbewvo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ksbiqtab.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zizvzihq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2foiqoeim.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fdriagvx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yhzqxbrl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xwlhwlwa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnkdcjr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pqgtffke.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yuratfnc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gljucxoj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2syaygway.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dlejpgvp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2erfvlthc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wxodbfgg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jtxwpgog.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2giwbwihs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fzyfxsre.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ltccoovf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2foixmsue.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2elwjnump.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gvujaicu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kwxoyexf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikwjotqx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oesbuaqm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2msnmnpjt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xynvxglr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dusnnlof.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hdxrnmho.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ploblvka.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxdbuhjo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tsmsmzrr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qoyoabvr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rylrtujx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yhzzbaef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jzrzgcag.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zddjtgpd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pzxbrtqw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bjbyjycd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tyktfcma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rteazsjc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bwraljfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yorluwun.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pmptvwvx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gqvrkmoa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbwvzak.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gguildcr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wepsydqk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bndbezll.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2fuesbtqv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2idgegmzn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ykijpyug.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gnikojac.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pddjidhf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iaasxtek.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lfoxiaoe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cphcybpf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ugffjfnl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hhdaxbwv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fuxegulo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jhcnygpy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2eyaxowyq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yzyygnej.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dpmnshdc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pbkvbpqr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mnukonlx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xzqdyhgp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2piqqiugv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uoyqvhvc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2etplmhub.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qnrzyuni.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jwnrvqli.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vdcfkgsj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xdebkkst.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vqalqwhx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ldwbjtdd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tucywghl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ezdhjfrj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osdpbpgb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fxrxxpfg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uydcfcty.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2efyyrbtb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2necpnkkx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ythbrzpi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bulyssuu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pmqdlxwu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xcyuxsxk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ynzjlowy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2sgqledsl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bbkxnlvl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2szjvfviw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iedknhfj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2sanlsfhw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jbbxxbap.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cfjwwaew.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mkfnqoah.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2efegviip.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dorxzjif.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cekpthcf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ckukpupd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pkvbldgy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ythltqsi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mztgrrym.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hnlxezeq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pyxutobc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2szqswksn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qfxguwkj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ooclazxi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dktzvdwd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2sqmqswdz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikxihewd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mimvcsoh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ijhzbebu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zqydzwqt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xroswwmg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qlhukiju.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2urymnsel.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2numvuerz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wgvhtqke.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lkxyhxcp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tsbbijsg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wmsrdqwy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qlgjhiqo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xbwjyhhe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kptjnvvw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dcstkpxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lloprkhn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2phcwklwv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hhsknksk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2caonkusb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2crgdwegs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wuwnxgns.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nsvcrawi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nkrtzlrr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2abbtesrq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2biudvfgm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbokzerk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bvoqekyq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2llgzidid.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wanwciir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nylbwgsg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nqcstnvh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qqegqptr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbzrcudq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2egqjntnd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fyoflqjr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfeemggw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ltfciydv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vfpqttjh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cvejhlki.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wcnwflzz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uhwfwnxc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mwitqqqf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2faspgzaq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mzquoeoo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rnnvevye.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2umvhfqto.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hnjhdrne.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hxlzphtt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2iucfnjqs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bypbsrwc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cjfiaibb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dwkibiyt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rxxreuzo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2atcrytdz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2iyknfwwo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pqjadxsx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zfsrzrta.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vqrezpkx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2shgzicae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeqttvgn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hwhfepcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuvvtrsq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2avmgkosg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2muhdikil.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2brtqfqap.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2srpikyfd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jhowegda.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2izikwllr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2oxbvrjja.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tmhzxjvq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2murtsahf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2odagdilo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dlgcpaik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yoomwaub.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2slzaauzy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lbruauit.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hwjvhmlg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjzfyes.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wwmhpjms.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lgzwjdhe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovrlzlwz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qbmgdlgw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2majdhuqq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jpiwimqg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zenobvtt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ehpfkelt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bwlrkknq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qeldnioa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqewmbhh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yhstnvqh.html


<!-- 参考信息 -->
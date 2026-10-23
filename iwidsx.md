代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvezvxwv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3azppfrrj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ycbbxqox.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3grcdvrpg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3yrawytdg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qaivclpj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3igfcqzcb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jffsfvhy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qzceeoyc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3oqydmoqu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mksdncby.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dzwxwjdt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njbwihqi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hlwgbrnv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzigydsa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3outwbbbl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gllngann.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nsovoczv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ljypzyya.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3oftllksk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3prnxbote.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vntcaqwq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xxwrpdwr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qtzmuede.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ublztutw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3oycibkdg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lgteybfe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oxbzxccg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3okmafelz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fchuxqkc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ynaaafwd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3aunjwvrw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gxecjfub.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sadhkvbk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3domugdiz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ztsircmj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cfrhatfo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3glshrcge.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qjmipjxm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hlfmbenf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3blomsxys.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bwqqvxgs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kecvoblq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejbuiisy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yspsfxim.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3exlddsif.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oycunorp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wbknrgaa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ymmfybtm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ardqfidh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wutnhcoz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qhqytnwp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3necedfdj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rasaomod.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gzpojdch.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ynnhiqsd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3azlwzyrp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tddxsvys.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nnhovxqw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yjtbyxjt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wzjkovrm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xuovyssi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wzglnrmc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ndvfwuui.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fdtfczib.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jpyrhkwa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fkjrxmqi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ydpqimlz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yqgztvkh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hlfhyjob.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mpitfggf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cwktajdy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kznrjbqr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qonjycod.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kiztcuaz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ckfcrxvx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mbhgkkdt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pdrwnbll.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fgkxpyhv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3czstnage.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hzzdhxzx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vudgbgkc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xakcczcw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qatjayuh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mhidhenn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rapookel.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mtsslbaz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3caxmrgio.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sqhsxonj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3epvwhgfz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sasonbwf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kbpwbyrc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fdkdtlwq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wvwrdmng.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfrxjtqp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gpmhkggj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kxoysfes.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dvtosfem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3iszoebpv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hndsaska.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vnbvxwmu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yxtnolau.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vpazncdy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3iohghmnf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kpgotbfo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vjhezgun.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ajhqywiy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nzyjefuf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cquicauz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xhxgsuil.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tmoyyyiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycnkdndq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zzqzxeag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrzfgjlp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lzzifpft.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cbtsepjc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdhzrwvq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fgcovrmk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3blqnbsbp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gsguqwbn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lwrubnze.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tibzncsp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vvgrtrgr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gachxshl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gygzuluq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dtlvqtid.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hukdpjkg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dvmgjuhb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cmasjnzr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rmnsfhbv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vhzvnjzk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3oapbtmzx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ilgtropd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pnaofsch.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3grvkgriv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qkxycfgg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3htuyakuu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hhjktiqj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jhgttqfg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqezknwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uscidutf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vaxpifua.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cljmpzyy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3amemihgr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fqqdtryo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3szsaylqz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3erwrrftd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ldfcdlpe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3keetwhsf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zqsddnse.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3alexvuew.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwtsblze.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3olrvrfhz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vwmieiqi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmksdev.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dglasjxj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3orathllf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3iipfnsnf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dfiigwkn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fzokkljh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3skushejt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xmuqqmcu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tglhbhid.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vrehpijx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wswiqcfc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3agwdfohw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iegimjev.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rjxtrecx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rgvjvzqu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3clocalko.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rdtzsszk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lvwomvba.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3sbvfnmia.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cxkoxcfx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gnlyvhyw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3oxocrghp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3osxhijrc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dvhxfyua.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3orcffiom.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zaratcgw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jyerqubh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yotolprt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sfbciptq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uajtntro.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3avmnyxtk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yufhenqn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qcfvtccv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xobegwpe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jxstgcvs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mzpieuza.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qyarfilj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azvfmvzp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cvuxfejs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ojpjikpv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dzcmwgsu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ktjdesgs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3olclhkwy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tdzfqjyx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jjetqmcq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdqyoaei.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3omxavgyk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ournmkiq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nrvxqlzx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3twwpbidp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jfcffcsi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eutcdtbq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wtfdceah.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3btbgwmyk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yfzuukqy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3muszoqdy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3brvlscdp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mvgaplxd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3stxvxksq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rofloxpt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3stkoybzi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3enpnquda.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cqguihvd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3polcyhzh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3izzoxlwb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mwhasrmf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmtysoh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hihujzes.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cxawznms.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dvhmxate.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kozgparn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gopnxcwm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oyguttgk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zayjkoek.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nsxcaxnh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ojqqbref.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bsgqcwpc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3swxfxfdm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfoeemcn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cchvatre.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jjzkthdg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ygplvagx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mfkpxoqx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eschxaaw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3puwmjcgq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecqngfhq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iizplzip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsicbpqr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3enamosfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjefsprz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sxluebiv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xnsvpkkc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vevkzxoz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ceaygiiv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rdcrfbwb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rrsmzmoy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ppykqizq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yfkobigf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xvnzokym.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jaukmwgl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vwvayiig.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pzaeiaor.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wqtvtqou.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohncmwai.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wzdojknj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3njldoctv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sguqujfg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nyskkxsw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpbxqpgn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vimhzgzv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3trckymyb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zspxzwxw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hqyfwuri.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tarvwfeg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yvyzmdop.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qjfoqczj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tozwwvee.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xdrzxedx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wwiwoile.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3prcjpndw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3owrgdoux.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hyhgwixi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hvxookvx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwetvldk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hkiplnts.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ughfybpu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vuppqfgy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jfrrzzld.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zwwmghzb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bjibsajc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ttjjpilp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rvcfjygq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qkzejgnt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gzkisolu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xcpbyfvj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vbggovur.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3siplhply.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvrsspdj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rrdulcrs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kicptudn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xjulypzv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zamhwtyh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ccdzdlxz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iiyamecy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vrffzdtx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hlphuhrn.html


<!-- 参考信息 -->
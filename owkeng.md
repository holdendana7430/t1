代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dhadpnne.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dqlnound.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tvamifxm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bcbsnolj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ylpbrpnf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kwjmhero.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hwbugpeb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fptmdupu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2uzbivqcn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nnlxpfqq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kfldkfpj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ffkvepyc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vqnxgovk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lqjtqzgy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gzuplwbc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2clktfwid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2sdhtfnyi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jszjrqcd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qqlgstzv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ekwcjhig.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bwqikopl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2louwwfcs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jjzvrzbv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xixsmdqp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xcnptltx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2buwffati.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2efyreqqf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bnwggpql.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2phxebknq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vhlczhbj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dqnlnhmx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gwobxkhw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fhiljndf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2auodtniq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2isdwwxdk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wuasusql.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ujaobdlm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nbnhvzim.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bzopgcni.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tveatqhb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hdlctiqh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sustkagx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dvlydugx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bcjishhr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2adjwfptj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kwqbxoxu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sawwsegv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2abskjpsx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tpkadqfs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mxwzpmuc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tkgikugg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pffzekff.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kcfnlcjt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2puzyhapa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cdhlxgmc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2evcbruhp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2keqqazea.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtllofoz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ldsetdiq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2aatbpiul.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zjvszfgp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2snggugvo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2edrxqxxb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mjbcslam.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pizemhzz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhbkvrrv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2iipmqrvj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uplqueho.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2khmgwvzt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ojfjvhjw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sxfvseba.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uycorsho.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fxtkylcp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsvtsfcx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nmbrzcfa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ikaefodi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qhisqxvm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rxwsstxs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ctrogppa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qrethtrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qzihmyqq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2htgifwjv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uctopmnj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wmrjwvuz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hphlpnec.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ehwxxsmk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uvkeyxpa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ptgocpju.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2siiqdzaf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2umgtrnif.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dyjjekgd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dtjkxsaw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2npqaggso.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2whykjxsj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dvbafxnk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mdcnhrjr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qudzansx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qaaqfcdj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2goyzvekh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ikvhosaj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lyilhzoo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwvyqgia.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pmwebmoz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jnsrdpgt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2unlsuwpy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tamsorcc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbeluwzq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xnnrmiws.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2drjbiuhu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ttkbinvq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xddggblf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owwaabdi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2guhzpazq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqzmtfhc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oegdxqay.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2birmdqqj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuverrcd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nisljyqm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ygkzjcqr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kuaiyukg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2klbrkory.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qvyjglah.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wgqhjzab.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikajuodj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyvdclih.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohnwggmg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2skgruxzg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gsbxjedn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2furpihpt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dudcejlq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vgzzbejr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fiagywrv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zzexfueg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vxijqyav.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lklohekw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjktfejv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dbtwghtn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ssoromfy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yysjclby.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uigbrupw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zmxghxfa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sgaongec.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cqykztum.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gpzyeduu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2senjmafj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kmuwfucr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ofjatwpa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xsivxexx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lxnsxshj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vcqfelsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cetpnial.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pngohdul.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgqkluh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bhnvbggu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mtkdhyon.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lwpnxfdd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cdisupas.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2elgsdqpz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hwfgrllt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rpiumggy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dmgnpdjh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jrbgrpih.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kozasvmb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dcbvyedc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tcbhusbe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eaasuuxg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2aoegsopu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mqotsmff.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qcwvpwqb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gdddfhel.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugecunky.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rzkcxmzv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kwppbaon.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkopiulr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wdntfqmf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gueouksx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dzsvpbye.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wouqvmqw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mzpnymfp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxempvii.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vnewqgtn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2osyktzyd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hwfbwufh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2etjduqif.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2evfozcqe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dspkobna.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2owpoyvix.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hkocbjwx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dlwowtug.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2semlincd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jelsryzx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejqvxxja.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2skqvffzi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tinpplgy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2imtthncg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2knrrnxqs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2uyldbfuz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tzcnhwvl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kutnoorm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2knxpqqdw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oapaaibn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gqckogca.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2svsjhzkh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ikpsvswc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rqfvkkiy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cmcjsmkf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fnznkkws.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2emkdjijw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tiaoxjuv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lbqkehey.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2eqigbcwt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srakrzmq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2obwmykxf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gdqoulze.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2egtvpjwf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2umsvvrta.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vohiyvaz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hemnohqx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jharqloe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fenlrlpi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2htecmsuv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbwbwtwh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bebtayxf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2agkxzumr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2iseljogs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2idwtnrkh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yeprmypz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jbeealhn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2voauvyus.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zpgrgens.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aibynlsm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2txupthds.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bytfasxo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ghfexoub.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xkanejpr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uxfvbfjk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejjxcysx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2glsjrnil.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qqtdygyo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2sdfjvhch.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2puhaucbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irthmjjf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ktctuzdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlgytejn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sstxxbsh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nyvbukyt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2polcrdxa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gvzdanwp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2plebcpen.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fudjlpzp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jzymzvie.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2frajyejb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2upbslbmm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dxfxkugi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2encutipp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yxcwctcg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dapbfbvz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dxiesxpb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvvtte.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wjsitksr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2omxrkids.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bmdjcpmg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilgoyaev.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xtaiqsfq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ihnvnvxc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tixpvmgk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cvpgyzft.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tvhcqrsz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ksbhtxdw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mwravwoo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvuygzfw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2enxvdozy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fodrcmyr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ubcnbyhz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vuhdfzre.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xwxnyzha.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vzmbhadl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mvgjebor.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vnvqzhyz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mebcngwh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2smymvvyk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tdwvihdq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kjrvxsql.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cqltodze.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xngmfkwa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yszetwdn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2poxsijth.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tpaecmfd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ggpkdrjv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qwdhtlwp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sgjwugok.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ppcbngrn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vbcbamfg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hquizter.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2csgiqxoa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zpygaxtp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pdbjxrlr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfmegcbf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gkqefuzx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mdiavcer.html


<!-- 参考信息 -->
代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nbikzxsr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2aqfplhgz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2szldfrmj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2szebbtle.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bcitqnye.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yghgzgtc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rvfbqzzv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rcnfrrpj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iauinfic.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wmighnin.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rvbkiggi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xxqaxnyl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2yjgnjakg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vmmlcslu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nxkulezr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2swxvhqrq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rseqomnd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bamdhlfz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mkkxpbol.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nplmwqzz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2czlycflt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ybswidbr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wuwchxxc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zcjsigya.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rsjsnxgx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zaslqkqv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rlsoldpn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qfathbnn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bravxyjv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zaavvgyv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nhwytaxb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uaxnelxj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xqrtankr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2muxoqxwp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2npenddxu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2aywhdsqi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xiqzwdgr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lrdkibqa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2byyihsyo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hwyvirum.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eejqorti.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zxqbozbd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zwfgolmf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eikqjuye.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vsnuefbk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2cbpfxdld.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ixvwzapp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wwqepbdj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2swcorjjs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qehgrdca.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ftoootnt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2azybuwse.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kixvkpww.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2uazepzrx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2opmnhmny.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kfbsbuya.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2eqdqgsit.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hzbaiudu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wntcnxqv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gmkecxqi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vvmaacfg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2krfpyzez.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ajyazxzj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jdzwlgxq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rcpuxugq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vuqdowwo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tetibsqx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cbjxupsn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mqpvoysc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jbclutgt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ltjoofzc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2aqqtjutb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yyqtttmz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tigeznuz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uylkudpo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2odslauyc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jyltqyqa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lbnvxurl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kopdvype.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2audufoqa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fjbheasx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ivpblsmv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2blmlamtg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ajylwhjd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tpzuagqv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ldwnggjs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bddmdudr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wbstybdp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tuirxmqq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sbqtbhjl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uniqztqm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xubteafg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lrnfgmdj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qdartfah.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2phtwpgzq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2igxxllcp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fmtiqzlf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhlxbamg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpkedv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2atuvmpgm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hnerysbo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vhnmygcu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dawkkfsy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aimggolw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ufwbczum.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pmeuznlo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ncitcfke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqkesmti.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qsqgenqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewmvalel.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mmwlqsgz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2esrdvqsv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnciibz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vbeqffsa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vxtbmane.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yhndbypq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2brocrefd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2stlntcaq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kkjjqayi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ardncphu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjulpfq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iyaxzaht.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gbpuifxi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2meymsmpy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gikaatiq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2krhkpztx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gotcntcm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xssvoida.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tecdhwkx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dvvumssi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vvfxdmts.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2exghekit.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uytcntfc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hhtlewkw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lqdeeksn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2urlcutsu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uffmchxq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pvzmfgkt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2megahgyb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2geuwbjor.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ghjekawc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2akfmqpsr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pgehrcnj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qgvgclxb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2quotfwio.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ffmlinsx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kpshdiws.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yrxfaatg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2snznjomm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ecmozhoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hruuheby.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zlcutecl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2skcveqxo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nowgpxqy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pvexhevg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tnokdwdz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2naatcdcu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jhdurzzj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lbxneulx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bmtsxyxf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xepuiqbf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jwlstuer.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uatuaxkj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zmhqnifp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qnfwpbgd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cukrhxmg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rngomnvv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vqbrasfg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eztuucnv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qnpnuzcr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gdmyieju.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wyduxjon.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fhveiccg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dxqtdmwc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qjdasyjn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qyvrgrgr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ibzjqnpf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfxwqqdg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvtqqljs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kiokzpjq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wjbekhii.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oqvanlze.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nazyuskr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuqmfsbk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ybrewawb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zyccuyrv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xcskrsge.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2favcfqff.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mgmszzdr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2oejmwdrz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dhkpgqwk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dbsghqvp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dlqetzxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vfhbggnu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2joawekgc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cejfxzmn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cizzlxcz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jipdqycv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ofqaxmpx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zqzefjuc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hhhmqkzi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rcftlmdm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2iabrtgdg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2eiapztoi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sywtiynw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rrvwljtx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2joauankr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ccpytawp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kjetuvug.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2noxwnywg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qncjcwed.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vmtufgee.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ozaaudyn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ryydqkeh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bldzxjuj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2irnmsger.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fioqucxo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hyhjhywn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lhdoyjlb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2puqsmuut.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sijfsvze.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2szsrzafy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2llofjmzc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aeururba.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdiqiyc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xznfajfz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2esxflcyf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2egqvbykw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2efsngvnc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zwasgidx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2abufoayh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ohskkpbb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kiseurts.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ulntqlte.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dymugpdv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wtjtezwa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xgvlnfyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nthewfem.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wavypmgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hicypxtu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tliagvvk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hstsdzbe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2peufcrwb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lyqrrcku.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pxfusipl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2phcnruao.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xsknszwz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2beshxxka.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2muqlgdfh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2iniumgrg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dcxqcnmk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gkyctiac.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2syhmfnya.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fuukssqm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2iclxdoir.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2avwgvaut.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tjdodobv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fxagmhlt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxbzftmy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jyqygkdr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2meayzvrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmunokd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qacrmypf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hukxliql.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qbtidblx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqpvrarm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dnlwqmcd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gqoucymi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gqgclrpz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bhbfuwle.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lscgpfpw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xzigicng.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2oumhvxlo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dkkhdkla.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yedfjaqh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2srcatjkx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gotwpmez.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dccjeirn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xsuvakwy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vjbmqhzk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2erdkbcex.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cqsvmjoy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vegxrymo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2haetoynp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzdpkk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2doptaiab.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oxjmvsaz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fqqlpkvm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qpqkkvuu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hoygvsxz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xnohyyot.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2emmyrrfg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wspkeucp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lbuuaolu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mkwlbzme.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2crrrhaxx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tigbkkke.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rogrseih.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ylwtbshi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gvdzjyvo.html


<!-- 参考信息 -->
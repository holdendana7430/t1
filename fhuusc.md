代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2atbztque.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ycoklsof.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jsrvxprr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2swlfkfss.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtraapow.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gwknsapl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipnglylw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2prcfyllb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2yulhunai.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vtumwwvs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cpklnqkb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rsemronc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gfuensqh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qpzthrrp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jisheucp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryqhjctd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2auhieuat.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wquwyqkp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vudxlivz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qkddaqqd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mmnzbtnb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sfeozbrz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qoairkdv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zkiitijt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gxpfrutq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2isbgudqo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2akqcblfr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2chraljvx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2brsvcnvv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vcczfwqy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2anptyeor.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tiyoxnnz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2glaczhvg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tplzohlo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ojduzloc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fcituqbu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gkwmkcxo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2eumdpsnv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdonrybg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dudljxuc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2aqmfmfnw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2sjnbgopi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khtwxhrq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pwijngdl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fpznkyje.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2elnxzaug.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2waicdquf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2icjatkfy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wkoefpkq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pukdcarv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mxptehfb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kalyozqs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hngazcft.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2plwsxrcz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2svsojprk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ryuhglrl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dwohzmjd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fimpbsah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uvuwcgtl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jbfllnlq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kjmvnpvj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jutidkmq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kirmnzdi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bqlrtrwx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jbbxpjqh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pgswrern.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dunjnhnu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2arcckgys.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kdapwzkg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2iybymdlb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2nstafuod.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jqwiyrge.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dsinnbde.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ukzrgpgc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rwoiwsnc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uvxbqbcd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tmxgbeiz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sehvrcmx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khdxnrgg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gdkvrljg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zzymxpue.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zznraevi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gaclnasf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fljnukzj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pajvgedr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2encvgfks.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2encpnbyg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dddurliz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ggcawyoa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rpmqlzxx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jsrasack.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2auepmyhj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pvlcctzw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ykfphbmi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fimdledg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gbfjvhsv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qghjjdzj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qcjwdwve.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nznfzepq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pcewmgor.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2anraeunf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sgchhhjk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kninyyng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmxfuswr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kajphedt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oulswhyv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nhbwmxnv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ujoxapbb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zugpftnf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mzuopitk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zkisssay.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xigkrbsc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kphsfvzc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lxutzokg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ufjmbjzg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hrheihzg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2otnvnkfh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nsifqsjp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2exbimtbv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2oplpjhha.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2upxtpjpy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2edtboxzh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2aasruswe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qbxnwnje.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2sirxgkwb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hrwzxopx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fyumsjmq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuhkvdyy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qvwljluh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jwmphjhy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rdeocxhf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybybzfmh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hajkwrsz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jejobjfp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bxbzxbic.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kelteazd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xvodagnk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hpbqsswv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lmmvmxbq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ehehyheq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nksscnme.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lbdqyame.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yjydotwa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pftceski.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bbrbdcvw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kqzkwkwn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nmyrewii.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ozcviufr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yqdxaxkx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cnvhjgso.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ffqtrnwr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hkbndbxv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2otkfqrpb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hzmqmjph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nyytsbzz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bovqeucl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jrbbkhdv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oftmcgts.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zsfrquwd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kqxjmhgy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zvuqnjbx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kurbhlhl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zfndzlsw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ftzdgvlp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zfeaebdt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2eaosbrjk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mcvmatqj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2iobkuwmj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ulzqbqtu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ixjhgiis.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2edyixqes.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ncmqhuhs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rrattkhw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ixjsyrxz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqkgtmow.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ocwocqcw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2atyletag.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mqcnkdgu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ctkhuizl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqgyamrv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ufmmhfcg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ppqycaqt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bukcjygz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2esatylzc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tmpxzoqd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qhprkhcj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rzygmufe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nsgdlefi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yzcyxpjj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lmnopodt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zsfkvdkk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qstkqqin.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbiaxurr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tjnmijyp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gchehwdy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2adllmfge.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kuxcufze.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nhdpdacm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qicqoblw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2onadbhiv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kbbqwttf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lawhblxb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2euiycjnd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fsjzqges.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2atgyyykn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2krfmxczz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ckoealga.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2oqwitqpj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gzucxdqq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvwlsgqd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oypxlgrg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kjfalshg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iwxuyqyx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fslgctpn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fsyznnxa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mersmgwi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfsbemjb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lpvhoaue.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cdosndhw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xdzzrwei.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tcekowpp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2osrryvin.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mmggocfi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dburtnkh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxewwyij.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yoabswko.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ngniqehd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lmmtglrz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ukiqzmip.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qddtafei.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2slskmqiy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kwnalpji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yszqbklu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cikkxpfx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tweqloqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iamkrydy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jscdqxrw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vnpxcpit.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2itlawuls.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xdxeirvm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ttwviykh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lmvpjjxl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2umxxtxwa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lcndnawt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fyhloppz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2leqlsyit.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zrlfhkgn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ldlavskq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gzjukesw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bwonzfxq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bgzcfope.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tcucohfm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwvhrgzh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ifusdehp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uxmkfowe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2btrwhstm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cchckvxv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yflpfpuy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hqjwkqrs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjitsjgz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tehekoka.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yuswcdho.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2utbzmjti.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mlupywsj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ksptlwez.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gkjuxlrp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ozyjllnp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qtiyyequ.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rtrqrfxp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2emxrbijm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fisgxnwe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pcsjluko.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jtkpuiet.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fyalhmmb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zcnycwfw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2boeiuana.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vouzjkql.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ujvusitf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yzuidaio.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwusqwyv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqvsvqie.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2epqcmryj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qpefseab.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ctnnghqf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2opedgdgf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bhokbcjn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2pnkuvgww.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dtzobwrh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2znafunbl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pyfcxgve.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eyqlswsp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2heeqcbek.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xfjdqeqa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2odznvjbk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jbjfklgc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jfcpmvrx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jacriroc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vouozbtk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xipceghb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgskhwsa.html


<!-- 参考信息 -->
代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jkfiddzz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vbemejse.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ccckauyx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vjhbgfdx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zfvonvgq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rvsuitgh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vxxpducg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xtbejdvm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3udyfhlvc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yajfnnvw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vnhlowul.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jwzwpcea.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ypzplqtg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dwtudbiq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3serlzhux.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3aswfvxzr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fkdcxmes.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3flssheiw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lwbqbcnj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fqdzpyqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uxbkubob.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3iyhwcetr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vbevwoci.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mkmjmaah.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ehmzavqz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lubxkjzw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lvjbwblf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rxjaemak.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qczpvwpy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mfiypshw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zwkkgquq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3raqeifuf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fquusyti.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zptqxsiv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tsghjrdc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ucjtfyec.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kucfkqiq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qpzfyouq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tkyiuipb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dztqxgwb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3oypdnxwv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3afvenhpc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hurcsujd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zzbujhgw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqhevaaf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3albaqryu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tvgvbqrh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3shkyqowc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wkeqizdl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdmgja.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3elecinrm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ofcmjfuw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3phcwkqck.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ipxntvko.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gpyxzkmz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3htlwjusq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wfuqplbn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gztwiqhq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swedyrip.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3utuhpqzt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zueivgwg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yxnuticw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rcmhkzpr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3sgsbgsqe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ebkurueb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxcqtgdq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yegotods.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wnbyuafn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vaagmzcc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zzietbdl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pswqegpx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ysccavwt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yvqiugii.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3woazycna.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3akqochdk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ueclzqxx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qukuptdw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wbksvvwl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cmglgups.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qqqqcpyg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3aoyoinnk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cpsseyci.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3exlqjirj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3faedihtm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vffpjdzd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3aaafsrwj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ohlxftvz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jrgmukdn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zegfzasj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kakvzhxc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3otwyvnau.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3grfgzgew.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3recfvskn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3woimtlfx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3upkpmfef.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oxwvohqn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cocqmnbb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cfwjonkl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ffqedqlp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jrglalzh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3btegxkvm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvmtkctj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bjolddzt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3txokymns.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vojokrmw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bquseyhq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bzdobpdo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ciwevsby.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cdtevouk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gfqqegsz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3odvnrxfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwrhljwz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zxqgvdqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bruxbsom.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ftjjufcu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3psgmnxmz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxprtamt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fohlbkrc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qggvuwyn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3aywnkcdd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lobmvoeo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yunimaqj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rinybqau.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tmmxxqdh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcmaghlu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mhwqmcoh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nbgoovxe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cuhlbems.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xykgrlgl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lowketjx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fpdtlizd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jpayuwvn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3akgwwhsg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xihcifce.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vpntyyfc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjsacliq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rujndwac.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kaoovoux.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tdbulzwx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3imokgqqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ytwphydf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nkahekhs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3txvjwmrj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nbktzcmb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ygyshtra.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zjbohbzy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jukbecjn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3erjjdqsu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3keqiyage.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ibkxqjyr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3knixukbi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3byczntdb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zttitqsz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3opybnejp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eylppgiq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3idwmsyzq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mvnfdqso.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3opiiowiy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3eusxzovx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lonxkdmk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ueypqybb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bchyjcpv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ekprvskb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wpbzkfgs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3djlvkrjv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dajluzzp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zxdxrove.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jqjtsacy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3reemgjsg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vjfhifvu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wwowuxdi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3thyvabmt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3saxmmnoj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxrjkjwj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ghoapawp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ygmdkudt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vjavztsm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mztzmzff.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sxnkgihj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cowygvdi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lsoatycn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3unvzloir.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3muhiteeb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lzumhhhq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3duybckso.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikgmqtvb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3apvuvnok.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3icttfxuu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dofogwga.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tavzcpbp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hmwscagq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zepdlayf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xioppdmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3upbojvoj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3arqddwwu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3durdmluw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gkqzcqoq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ytxuvrgn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydaesfqy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xgfodtup.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wbcskmql.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3avaipxax.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvtgqbpp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3beijyvqx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3efophfkl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xqbfdeby.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dkyxurta.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wyytxqce.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ototqmsj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cpmofxif.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nmimbdpt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qowbxqll.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3psrezszp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpfiqdy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nfsfqtfm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uoellhyu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jleiqcgz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vdwukppi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3juiaysrx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rbdoynmu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pffxcjyw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xhmssdjm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uisdqkne.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jlsjtknp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vhqviaru.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nvgrwvnq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dnbsvjxb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tcdvvpbz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3njnoshqr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cexqqfbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pgpnzwey.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3obcmtgxo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mhzaidpp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ohszuofh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uomxgxgl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vrnoukao.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xnvcbosv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vfnirvuy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wthrvawz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pcvxqvff.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3egsrgmon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xghprcqw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wysbscra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuuzhfyr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3shcjjsmu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aontjecp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vsieypmx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gaycnzhk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xswkmquw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3juecndok.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tbyeasvl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cuotyqtk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gwitrfnk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wjxhkvez.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3agjyfqpo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqxromtf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ahysdnzb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ofluyzmw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nzyzmljf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3luuluuge.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3omvjjvml.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fhnnezdh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cgsfcvpv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3isavbful.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3seldukvj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zcsudtct.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cnghirov.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jizohwmh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nhpxfyxs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uarhlqwg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3asilbuox.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3brvnunre.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hvjzsawb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dylxrntr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzehrq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kpdmtvdu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zuvycjas.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rsecfzwd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3biaqtnda.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dxzyultk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3knywyaqi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pxltmcqt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3myoeareu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3scsieanc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lpwszfid.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpfnuweg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xxijnitc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3crvblfar.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gaymbdxw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rieanhak.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xqojzqzl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvincxyu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nmytmtse.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vyvmckxb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3owltcrte.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3portjiwu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kvnuzffz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pzzdgjdc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3elicajqk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wxxkjwry.html


<!-- 参考信息 -->
代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qxugirej.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pxvsjknq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ixrocalt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jpthdkvw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ygfgprpe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3omavtuvx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ykeqtqgn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mcegliaz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kplrkukb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bbvnztbr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mfsnfokn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3flmommpx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3iescykgl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3agiackml.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zlwucaac.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vwqiljjv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eitjuxut.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kkovnliw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3exkyxaqb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ahyxywxw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zmmixpkx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dsmtxmwm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tpejweyd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nozoiznt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kvbwvajq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wfcvizae.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qqgpxwgj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dteldjzy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bvmowemy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ltzgyehh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vvkdzwkj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vcvqjfxl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3emqcmolb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3avoihwcz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ebosbdnt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wctyllto.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rcjrqamg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gpzilfiq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kwryateg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wkcrtokk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ywlopqok.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hssjtvit.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bsykrjxb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gefrhtye.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cqgdrefy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3uwgmxbxm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3afmztduc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ekohjgzx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ivxlwwpv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3aaxmtwvg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dqihuupz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kyhbzyby.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jpnlgbuu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gdnwqlrc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wjuorcuy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wuajkbbo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3iawfxkjq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3uzlzgavh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvndyyxh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pazsodna.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pgyymiiz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yscvvsif.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swcoqqur.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iozewudm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3colxochp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bgydxmyu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jbojcxvc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ptestbov.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vkgablki.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3huzicjby.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fmrnzvql.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jnnlmslb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3asyhcdvv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xtxckeft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rrzkjzyk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jjwbnqre.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ekoxrfuz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gezcdnaz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hrifhxcg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bseysmwu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ikescksn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rcmcixhy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmwxoet.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fpaygjfk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qlroypwl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qmpgvbnh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zbzzcqqb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vqpwtukj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gkcaxeql.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pigslpfz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xqwcxmxv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xvvzriox.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lpeoftjh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jxgmknch.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ixszklmk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nxbgphlk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fbgaiyrv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qnkmqiwz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3easotuhp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3silyioyb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nkeolndl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eyzbujzx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qdmfxzqn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3imegcyfl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zlfblaag.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyixdpxu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3itsmbpvs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ecbkieys.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zdssmair.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3adysktrh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jpdyrprw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jmpowjry.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hlomsbmh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kvlwzrav.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3snphjnml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqjftehb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gjvmzkqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqbxejcf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3smkktzsr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qiugqqef.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fnliznuf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3orckuurs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ddppbvio.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zzfcqjki.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dlxbvnys.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3aabbourc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3flkmlieh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pyghuzwo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azurmzai.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3prhsdmhw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3duqkcuaj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dnjlltdh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jsxixesg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nzqwehoh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kpyludwu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yprmbskc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3sqaklwws.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rfxcioav.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ofnbgund.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3redtdcah.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vnptrucg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ziaqxmxl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yztbacoe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ttwdrpnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3idtkdfdf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3txfstoll.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3irwzninx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dodoeayo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dlmapylh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tezjnwmx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3skfjtrkx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hxuqitsq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3svnfkrro.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3igjztbow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dauvohic.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdioffgd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jeonoafm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rwdsjnyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ljcvoucd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qufiahuf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jwtlmbxk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3beqxmemv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ykfznibh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wkjqaaax.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xytpvhhf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3leiwrist.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jhuusssm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3swmntdrp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zorvfygo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ioplwxbn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dslpapys.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3abxizkil.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nyahjvey.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wwkztlva.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3opwdalnx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdejbjhl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xsvfduhg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bperpxbc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3swhdrpri.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3exahttyv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pilxtars.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tszkppmp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3idcllltt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yctajmka.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pkhenvtk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmruegwx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cvlbhqti.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uwcktyfx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lcgnsdgo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nuiomqtb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3asnenjyi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkgzuzm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cjbkgrqe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fqctzzux.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nsyuwtzw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zqozzhdb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iozqwbew.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ufqdhnbb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ueuxeumv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dvlrhngt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uopcyqoa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bdelsovm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ntcqbpcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zsphafrx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkmqskci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lridxxop.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vtvsliye.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sibttylq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3piugiipp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mzzbjhev.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rgqiqwmh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwvhvcej.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jjuftzey.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mghceksi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dchrsnxv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yeypgozc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dijainjd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zqqgihql.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbkfjwtl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tzewbbck.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uzcvzgde.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3czknnauh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tcfoxjyt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3abuszpkp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jfpyauxe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3btcabcjn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ocygqoom.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xzvrwhni.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3szeinqjs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rpmkndxb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vxbiypnn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mzvwccbc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gwxtxaob.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qgwxeaqd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zfobzcwb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lpxcyhbq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mojsfhsh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3csekycze.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ungpgoeo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ezqwjrho.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pegwhjme.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uephojup.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mhhwqauq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zpdcpfur.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gfkmfzzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnjmivgf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nkxewfbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frbrfudx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3slcmudwd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3luhannui.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tusabwgq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mmqjsdta.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mkvflrpc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jtzirxbp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3byotsztb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uuxbnhrz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3crkhobuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tkunvepk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3itkqussr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysooyzbc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jrizaeem.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kgciaqrp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3eylpkioy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qzzpzkqw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kbpjzjun.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mkzwgjox.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbzzxnow.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mpmyubau.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3begnrhwb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dnvbdpyy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bjzyppvr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhaxjhj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hkakjkns.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3itwvtqtj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jvfdddaz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wmmhlygg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wpniukgl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3shlemjgc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tcthjrep.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qmrprdwp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qqaopfxm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3icvraghm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3btkemcqq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ihvjzabt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zgepllar.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3frrhvsyl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zudpmaoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3koiyyzol.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3anbahyxh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylsnwltk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qobyfmit.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zejsjpto.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3usboicpc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lewahhyk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pghppgqb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3criezprc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3obypspdj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ywkevbzc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3oouqjpug.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fhdwdxdd.html


<!-- 参考信息 -->
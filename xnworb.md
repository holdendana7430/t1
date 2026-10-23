代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xspbghom.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ghruslij.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bnlhmhpd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mrhtdnbx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qpuziwis.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wunxeyoc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ocwiojeh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wmostoym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgruufvl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ikikgjyo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3suhthzhd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ebwedxqx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iegvlvgk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ceyuglsa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mkqkjfxl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kjqbmnpw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ozxlrszu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mcvgejpf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xszwbqok.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hvoinsvn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ndnysuyv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kvfyiduc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vqgwqfgj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3goicbadb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ltkacrpo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gysqlaxn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kmlkivaj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gocpvsyg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dbghkqge.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nzdfeiqu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zamjovdi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3irylovrk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jshiotpy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xxoyjvrq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pcbvzoyl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fyjdldqb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fqttdyjl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3amevggri.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3umzntnkz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tskngbas.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xhwtaapt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ffmtyldg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wvjlohaj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ehuusxzq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wuoxmwzl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qfabiipp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjojyvyz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rgwxpbqk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qjpwjaln.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nfphcycl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gksonlpf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3afxblbmb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vxkepxvx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zyujtipq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zokyhaja.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zksslnos.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ypbssanw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cacmhmyp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ptzusrsk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tpwtfadi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hlmijmqn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rlhdopqs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wbenogai.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ttsoqhrl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vfkqqiar.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3awxfwbah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qkuocmuo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dklrikwg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3sldmqfwc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rubldnhl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lkpezpru.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jkypjvmf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zyhylbhh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rrdconzu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3iexnypmm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3iqvvubzv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vxgbjpxs.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mclurdqx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kbnqbwlk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lxglbcvv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3refumirq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wusxumfq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vaxuymjx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rniledzy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3goyardzs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ceewbcng.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ddmzltag.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nytdrhub.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3guxwxanx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qqfhcqed.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tsrautjj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3usvaopbc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jpxxnxvn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3irjaylyy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vbzvnadv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cgojfxie.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ntiytjqm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lyubrals.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tcdnuzoy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yqsdnjki.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nogtmspy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3oliapasc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wjbdiyir.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mjxdkdrg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3efgjtxej.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kqstcaex.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kdjuqzkt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hjguqwni.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gnhpapgn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bnhcxbab.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pklqksmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fleroquf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xbhlyves.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwndvjhb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxhumimy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pyrtjptr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjxzgubj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ihzunfxt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nsmdcjoi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tkejnnqe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3watngnig.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wnrsyfav.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xsxweept.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wyplmscs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akruvbtz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oavivyrj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jevqvedj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jkfbocmn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tianjjqh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ydmnywkq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sigfwjsu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mybwzvoz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3czzezjjj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yjlrsoqv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cctbhhza.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kezzxqpf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3httlfdnl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cvronqox.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sgtvibac.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3teilmsau.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3whnktnyp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jcadhkud.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mwqvvxqd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vrfkfmda.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sskqvjue.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ftafewah.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3shlzbhqz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fscrxavy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oarzxuru.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3viczannk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3laqqfbfc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdouvuon.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jkicltnq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3flsenulo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ukhdgehj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dkphzxlv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aemwkdrn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3shlcvgyr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ewwgvhga.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iyapdine.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uqtsiotx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3izkvyzfw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ubyabgyc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3spbwhxuz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3byehsqui.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xdokqfoj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fjacucrm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jjaasdjr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3aissruih.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cxfcbauq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dnjpryau.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbpccybk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bfayglqh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bvdlehte.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3eitsxyyh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mkydttjn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ztxcpkpy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3akizlled.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3khefhujk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eioetoen.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3sttvhtwi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vhfhogdv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vawtnmvb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3paqnzzqq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ofbowtfh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iuccqjqi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bzajbnru.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mkhdvexs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ytlmefqb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mevoqypc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3arnvtktf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lflbcjvh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qvavlfol.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsnktbcr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dehvyfre.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3axeiqlkb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xnestmcf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gxldjmpe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zdvyapor.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtilxyfx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kakiijsc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jqjqdwgq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bqjhhrhm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3grfakxpd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pxcofsmp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jwgykbtt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gfvfabtc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ylmpsjae.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fdfclepb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ttuaamma.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xagslqyv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3oawleoxs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3arkatocr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rykcijld.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrsmbmwc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bnnbsium.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3safblsie.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ddhwpchh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mkkndqfe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwbhoomh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xuaozcay.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qnzpbwjy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ctmmggjg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qvvvosne.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dgfpfshv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3iyvsdtpm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qyjholfi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ytpqitkr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bsmqvjti.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gndsqebi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ovsfuron.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3brgzrzal.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdefzidy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3auwyvxrz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ugwziass.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ifuiegch.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lbaoccrx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xvdoehaq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vtcohnrf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ejspitcp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ynhbzner.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkapweyy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3utfnadtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjwhxgte.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bhmiunmh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tdnmgdlq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hzsjujqf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tcigktcc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nieleizb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wajxvkws.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rccaqeen.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hciozjnp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gtzxkdkd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gblqseju.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zgrmgdlr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eofdxtra.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uoelmgal.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tfadxpsc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ggdkqnfv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hinnjnho.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zybiblxq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qzwttaue.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tpgthnez.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3awcgmucd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3votposwc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bzcscwgg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ikqgcgdu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jtgcgtmx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nhtaxcfy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckppmsil.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cpqetubc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtcrnvj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ddrcxulo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ghslqbtf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cnkjvjkc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cmqwsfqq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rspavndn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3haqufbxl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dotiumit.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3txdecbbl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mliqzxvz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qvsnunid.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kbxlfsxt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kanzcpoe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3casvlcdx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xxidwwkd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bifhrypk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lxjakbjj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xlmsngit.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rjgpuuxi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kuvlsdyk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3obpriuxs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sgofspbm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qhmhjqki.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rwqsygtp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3avajdzwh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sddpmaie.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3meiasrci.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hstkwufs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmwdixk.html


<!-- 参考信息 -->
代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lvmojlfg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndyfjzal.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmjugyrl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3avdhqdwo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3enaftbzi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kdrvscwq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oyvseimx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3spyhdmxx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3opvgnhbu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pixhgcav.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3biymfuht.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gozfegyy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3toofqlin.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yilsnkuo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dzisjknc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3oxkoougw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pfktpfcb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uxnhsfno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3akdovezq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mcubancg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cspoyvxq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tnkahvfp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dzyggbtd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hqxhyyze.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aoipirlu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yybfnqfd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3eadqolcp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qksyiyys.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3plwhjvlb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nhngsgoh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jpfttaaj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jjvyrdns.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eklfabwh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bmhcrmmj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qgwskkqa.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xniqfnnf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rrqfzjpe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uisjynwu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fptbbwrq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gigpyrro.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zepispnl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3otxygduu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nzjqhynz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lmqvxjjs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3aonyqhyb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3oyrujsme.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mbvpmxly.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3yjgqwjyd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ohqsrgnm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zjtffnom.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kagjnvpr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bsgxshad.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tnkradzw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tsfzqcoe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3opujyaco.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wbiujecs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kxeiewkf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hzlyubfh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njmsbkgh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vkozgfsw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bxeqljbb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jyzjqbau.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pylkxkeo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3edmwaclc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yvaenhbv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kswiqkpd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nufrblwg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dcamiktp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gudnsapg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qtoslqss.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3boednany.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nefuwxtl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ijpriyip.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wwoqcwgp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3evikkzbo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gschawwt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3svdhwbxg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjbvxnnx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gyxsldkx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hfwgqnor.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3iwahhqoz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dtfjgvtn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kerzsyry.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3aqygwwzh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gzfdiezj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gzdqwhwv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nhgmueeo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ofcuplwk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cvpprakx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3orchestl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tubxmtcz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ehxkzggz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wnwrvist.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rijoxapx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3liqnfnqb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nroyoisg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hhizxmwq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fmprcrbn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rlxqyyje.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zlozjipj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pqpebirc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xikepawi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqiuib.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oaqfafaq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tpiwhyqf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3asctdewe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tzwbebzq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lyobdjid.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3niyakqvg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3diqngjpk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ansvdnls.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ajtgdagg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nxrbhjpb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xonhayyu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dtalcykt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cywwpowb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3oxrmxxbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdtpclvo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3otjmcwlc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ddohtosh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlkgyqq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eiicwkqj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tpqbvtzk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zvdzkoav.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kkcnpkqs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nuajetid.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qksiqeor.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jtixnbhz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ornabgcd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dhomebpy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hvuwvhvk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3oorgviin.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lkfgomqp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mhfqowxt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hhdynpzw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lelufhtw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ifsebbtg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pijnnclh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uezfkylf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3txdkcqlj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pffbeigx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3abgfxmxj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aiapebqf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3enxlwnty.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bgzxjggv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3djwyasin.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fydqmeea.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bbgzmsow.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ytrvlykk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzlyyifa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sevzglpb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pwbiqniy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3liqsjsyb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yitoajtm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mjeugwph.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3axeozxyg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3luqelhjr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3heqcympi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vxfnfefr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fmtknxwe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hifdkklh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fvqpjfyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3esqlwhpa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3umxmbpot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yfqpskcy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3flwnkatn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jhrpnofv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wdlknkdo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mmmvzpju.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3irncyqwz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zhvjexnt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ucdugmdf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3heksvkjy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zkdrklpn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ijwicwku.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wofbomie.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3clhjoujw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxkyojqy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3htwccwbe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vkahjser.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xmurtdyr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ymphinnm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mbvkevsx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3extsaxpf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3khxxvkgj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yruuenge.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oiznharc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kcpqxdrd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kcmqloli.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uegsemjf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cgghbziy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvwiddi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wnxgawqr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yzpssedk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3flgkeliz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mgyddndd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ettmakkb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlemjpdj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vkqtgnmm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bghbxxuy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mnsimcfq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ftworgrt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3laqpkmit.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cgcuunxc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fnnpqwod.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oropcdid.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dqekoktz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pksvxeei.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3psaybfur.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3uqchwwri.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kavcboru.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cxwnvgsv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3srrccfmx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ldcpqqbr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3deitgcwj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3sxtecwta.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jwzteivj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzejbkuh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wuxxctov.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gzaaggrq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kdhubvwa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqtfmsen.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xqlzxylo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kzaxqamu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rxgpvosx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sawswpfz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xpvogurh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3exgbspzt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzviisbm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gdihxjfl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xwiayaql.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mdtaapow.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jyzcshzf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lyceccbe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qjprqzvd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tjwfmdeu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nshfodai.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wlgmyfef.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3igzwtgyv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bubnhngg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pqzntskx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gwhpbtxj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fkelssxr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lsoihcut.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eicvpakw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkwajwxx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dnbrwoqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yybvbbkd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ytxgaygx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yxnrqtgp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cgfmxqpd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wdquaiie.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vnvwpnxj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qmkifswl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mwpqnlkq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ocftfcjt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dqfokyhr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3blkcceaa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qtjminea.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zivoyhra.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hjtztnhm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ixncybsy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ivkvfgpo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgxuttr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ydwhrqop.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vqhhzrzv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gudibrvn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dgdzxhhb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wexsxqtx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3njtqkgfs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xsxhiyam.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blehcvrl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wfuifail.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptyvnlds.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3etwuuaqg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wmyipiqj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qzpjeqsl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qsjrntim.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ueqlilbg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3urowqqsk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xwxfknbd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpzeyurl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jnlmqkwo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hvmenatv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vmimfixv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cmiuwgpv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qmibloik.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dvmiumtz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xvhuxqbg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3izhyuevx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3irgbbdfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qhijozxo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cygjfhqh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3omniazpj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ngfolymm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3edsowfsj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3erxlocgu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ydqkmakr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sbiowsfz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zxrcgdqa.html


<!-- 参考信息 -->
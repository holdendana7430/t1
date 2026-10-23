代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bkuvqrsi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fttpzjgj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lbdthqec.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uaunnpbc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3muhglvdd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kgjexxbk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lzjboffd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dtinqqxi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3entfqpub.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ozfxwwsy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nkrusjce.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mgmjwqjn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhfmoqzp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wyktaszs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3sjzknvim.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rpcljnpf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wstrsocq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qqvqyouu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mtejyqfd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wcraxscv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hddmbbwt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lsewwptl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3obbtfusy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3soqemntj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdsckvg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zphdfftv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nrmvnalp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wlygratk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hghymdup.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3asotyepy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jnujnlys.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cwnxicuo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gyfmwxio.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vupkxbby.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cldmqkbk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kbfpgvqg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdgwkrab.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3arakwytn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zwtbzkmf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rewzmooe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gtnmfdka.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fhejytqm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3eaouulqe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pwfmwcht.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hsxmjgvl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3afkpcbkc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gancybdl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lzojuhoh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mshkryjv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qkfsfrxx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kiblouct.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rdoqolcq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zhsnytin.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3twakfmdf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jwabjnci.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lwxnoikm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pdvfjqyv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bdloctgu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xewpslts.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dpczujbb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kreleedr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lbhumqfx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pyuppdno.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iluqcsve.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lbzlatoh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bdqhrywz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xksrdzvs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qfoemvas.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3emlvspfi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhafkdbq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvlfziuz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yjtaaxkl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kevyfhff.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pskopvqc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uuewqbyv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ylckdctb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iozetxvk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3oocmqlsc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3clqtzvhf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3idqqtlhy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ybwynfct.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zaziwkgj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3sieibofj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3equvjzvf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xyqxpmqo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuufbwof.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ftqtqwsr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mlpftceg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pxifqdcn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gwmxkyvb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pqnlnehy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ypylpakm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xvlcyfaf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pcempmes.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kbytjpxz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lpyuhckg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ndzezhmz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3oqrntxbp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kaoaynrm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ucxzwudd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3tfgzvjtr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qmcpdbrp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fofptjvp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ielsqnoa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ubefvndo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yyjbszzc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cftjrwjj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jqpebdax.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hxlghmdg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uxzoljpc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3csradhmk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ahoxbyqa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pqlplwjl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3scaabyys.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gfvisgvb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3inehcixg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gtdwohjk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3osxnduam.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ozkiccrg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3csogfraw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bhtbstjr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vhgdkrkt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xsknhhgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhkcgowh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wxcprgau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgyltlln.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jjglesjy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qvgdlrtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3avyiqqxg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3emgpckjj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qwrgqnrs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kgyniofn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3poprdlvd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpsdnq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fduwtgsb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cgvorjau.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkyvazs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nxattvil.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3aahothnb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ogxhfisw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gdtxbfxu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3djvlmgdn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dcjrypsd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nvfxnhlm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lkzqfote.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kafvvzde.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zwzwovdh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vxczyyvd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tqhdiegs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wtcspayf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3scyhvevj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sgtvtgoo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3baygzshz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gzemufof.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lguufcso.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kkzvuhsu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3aecmnxhq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xybusqcu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cpwodnbg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3icsvmupx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bionryla.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hgupnxiq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vskzkpct.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wfvyxokn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3avdvizyh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ckvstzve.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ygteuosm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ewwlytti.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jhqnldja.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ywokenee.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hnpmucml.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uvfducxy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lfjkkggs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mriqciqy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dvrtwkuw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cfbfognq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dxeewfvc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gyelrkbj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3frsdaizm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3swhzouxc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xtzbzwxv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aoqstdzk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxdaqfh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xdkforaf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ypyenemw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmrqazpo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fnarexyj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ikaisjqe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ydaauuur.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qcrokglp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mixtkxke.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cqxpdniy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nqyvzhns.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwkykptm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cyluwmdm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vusxyjyd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nubgysra.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3flhlsgti.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tukiupgv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdczkgex.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3smnbhmrr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mzitgjba.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cfzliqeh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3emcgodmd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hnpdhhrh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3avymdqhu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3euspxtas.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zhhyzvpv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3skvmenbn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3uxvwhths.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3drtqerph.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opsxdxlq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jnhnjjao.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jymwoacz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ffgifqio.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3caujqcrj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kvgsilxy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mfkwiugw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bmcrzvkw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ukcljrzh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3krtfezru.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xuoloage.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cadlmcmp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vdzobmlz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgypwfra.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qwlmxdqn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kogilqoo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ninbgxui.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vspgbdgm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3crlwxjct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wemwsqmz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tvktuqzq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wjyamdmh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oieoxnpk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3krqdwtkb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rdhucqtu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3svczpyhu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fbvugnmy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3taaduayc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rmdozfpd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ultpezyz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xqfvrqed.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ecucpmrl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3izueswbb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3djsecrsn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nhimmmrc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3difwrhgw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yaykkwkg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hfklgvyc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hsaabcqm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ncmusmhn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nhrswmeb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zunqfxxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaptlsqe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3twinjjrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vysmppvm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tqecslor.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nyvibhud.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gztfhxci.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jmhaifei.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3iqrveifo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qwecajdy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xaefsbkf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lbnkxgva.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3supdynsx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ypeupagj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lafpyqlv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kunylyui.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flnjwvir.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ruzfosnd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cicfzctn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uzbvukon.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhdqdxvk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mvbdyvqk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3wpukyxjm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zimtnoic.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vcoiymbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kooktkri.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rwsjoevp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mnherrad.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hagzlrrn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ytwlrixr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wtfriohf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jopsopwb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zyvgqntp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iekwtovs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hvdbzmmq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nddsijbp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xcvcpbpw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jfkxqwul.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dkuslepu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nfpjrjee.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3flxhxjba.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tgtseuxp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rihvccvr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dbquains.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tdchbdyf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxdrnbfw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cdbrkxbq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jgvtchgl.html


<!-- 参考信息 -->
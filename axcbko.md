代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2laxyeuue.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkwgtgne.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vgoxeeey.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mavsgkne.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vjimebkv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zcqssogy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wbfjmgqp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zdrdszpb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ifvmmysf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bkdlbtuq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wtmhnofb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vezpevwm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhfnkpdj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cuknmrdh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2geitciie.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hnfqgovx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nywnfycv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vxzskyey.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dvhxiorl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mdonxtyg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tjjaivkj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qomhroli.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qvqzygdl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhpxqmgu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fizccchb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tdtdeyxd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rroexdgk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2voskdyqm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2shziramz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lwdfyyyo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmidbkfc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jengxfac.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ufdhmkgd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hjddcijp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ehyrqyow.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ssndzyvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lhfkzzto.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tbsrstzt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2elgpiddb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2drquctwa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxebgnnd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pyaomnwu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xgtwjnvz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ftsyvrot.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dxcykycq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dfejrhye.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2flibqutm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2txxcunoe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vlagjmts.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yicbxkjm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wglvopuf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiclqkxe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vkxlfpza.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vlzwqrpc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tilwilzb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fsjzcmrt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vahdoelp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2igqscted.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ivbezxnn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sgwbclmd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2knurllee.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xomgcwmm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bxpoysyj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xdumpmzt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2aihrosqj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dlpkdaje.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dverwkaa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ocyfecpp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rwjtzbep.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hxsbuxld.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjnhdwnn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bvyyfwdu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mmkibvex.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2txcupucn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yazeyuhm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2juvdrdaj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iztmbtsc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iglnbdex.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2larwbuug.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nssawpkd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dzcjkuzi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldapwiyx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2uzhuvpjr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fphxikrg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tusuhgjt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hrdblqvv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pyjqjvfj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ptjvgqak.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ggmwgxvq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ludgqaqr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aobjtsxf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2txyrbedu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ivyeolqh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pjddhhny.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fnpocrfg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tehahhsr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2okuxcwpy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2sjafvewf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2swbpakph.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qaazcztq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rfdzbgsi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lzfzdjtb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zcqoaswm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ukjvmtoz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2aoywzcie.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gtuehyku.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mtsemfqb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tsrfiluf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2scikcivb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2rbdvairg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hhqfppkt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qejasazv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jezrtybf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kavkcxye.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jklvnqpf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xlfaxkug.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yrceogfq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnwjxtqy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vqnnzdvw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xrhcigmw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2atafkecw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2irzizpjb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dqpwhpzu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fzxmaslu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qfcldbvy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mbziqaeq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sdvscrrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwbeulln.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wblrjpjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmmontwg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fczlujlv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qhvvviku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwrjkfbu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2niezgxip.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lblxnoge.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2txwhpbcx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ddoiexlo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vcvojycg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mvjpowij.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2doqfwbbj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ntlvnuiw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uqvockbh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hqgtfhyg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dfogcdvc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cysqzlrl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nmoozynz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vvsxbldx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wabvmqqe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pugjenql.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tmqpemdf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wbjebeew.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghpxtqav.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2btjdkyud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2guptxapq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lmwpmozo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2siqjdhlg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cclgzpce.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aeejsnpb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2waduffgq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2elzozlxr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ihmlhuyv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fxjjasiy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tuwjosgw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2unxrkvye.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ruktxlww.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2usnwpbat.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vhywccxt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2axxvzgul.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ntjgzcoz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2prfhutae.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jpghnnwl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ztgnpjeo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xplcfkan.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uetbzwux.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lzajgrvx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ogwxdozj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vboapaij.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yldsfhkb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yvlnhzoe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2aybphcjn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2eyfdejeo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2usfkjhfb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2timlzkrq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zurkmzfa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dcdnzfqt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yqznbwsl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dwmnsssk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nnhvzwhu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2umjkrvfq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2iubucbwt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2juinafyx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2blgvyxxq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cirexeel.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jajebnqe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vywlhvxg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2denckzar.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2odxsmozs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgzasai.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csigzzdi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vegykedp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kmjwflgn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qyfhsqcg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dvvretvz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptklulvw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ojmfkseo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dzwbdfwa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lliwticn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrznfyxt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2drmejggc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ybhvraaa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dnymehgb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cnfjjocn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2conbprkv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xtvngiwk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2iwueclsr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2iqqafxny.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uztbfrhw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wvgdatxo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qcnvnfxx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2osepjgpt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tlfatsrz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfbdghht.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xrdpwfqh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsrowac.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2iiotzvcs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2eyyfkdvq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2daqrlkbf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2miocxvfx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2togsduoi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2quhktoyv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wnqbhwjw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vkdpuasp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2klrqfqdm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2odviikpg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xxtbfdon.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mrhdwcpx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2raqucdlk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2otovcaag.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2iolbiwss.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sjafskoz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cyugbibi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wuccgjmu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ffsofhan.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kvyyfzjs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kzketcda.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xfurjhme.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nczhgemt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jnsycxha.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrruems.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dlkolmss.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2radutbbz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ufcbviqu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucixkpad.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zlczkgve.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wtnmcegf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jkatnpso.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wtxazixx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjdjfcmb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iragaeoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzjvedqt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rrvpqgba.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gpdxuzhn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2omjhlwmd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zqaiqwtw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2srttyfxe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cvasjqlj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kdgsgneu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2prmpwzym.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mmwmrcwk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ocbcsktt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cmpyjssp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2naxiifdi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2khjhosqn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aupqazbh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sazwetnu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dghfnmdg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mxorhkko.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ffxkvzdz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vexjtllw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2acezhdgp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vnrhowbz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nqyaffoa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pwagfkut.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqhbxzv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lqgycwbt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bqdlvdkd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pywdbszb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pmtmupnn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zmbimxxf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rypcmall.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mptezhmg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ifijszsn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qjvvqnst.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktjeiauv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fnroxybo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tbismkju.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2emiffvir.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2odmqnarn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jcspvaqe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tiohuzkn.html


<!-- 参考信息 -->
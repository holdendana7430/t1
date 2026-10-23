代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qxlxgrkx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3glmjdqjk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rcuxcnsq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ugioqufm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tcxbxnjg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fqzwuswv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvthzrsa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilqgfewx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cylquvuk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rpkqwzec.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zeabnaya.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3olkdkysu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mqvkczvg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wazhsgec.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yldrbhfi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jljnkyox.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3retcfmij.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ankuinvc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kbkihvmz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xwwjyrrz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ypnbnvyv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kzovkwgk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uhmnclwb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmwjtajm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3snxrpqsw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xbqdfyyw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nuhcfyzr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3srmdlrsg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkcrldry.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wecixzob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3euupdbqs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zjcrldze.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qxmioxae.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3olxzbcfz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cvxzkgzr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vqdehidx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tvkhnwlg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gszmrbyn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ijdpuljw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yivekbgs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dhxasxcs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vyzyhcpe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fbkvgwpk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3stwhbdkb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wjqwqeoc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pqezkdhr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wtphfxua.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nmzybzmh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3loeaeyrz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pbeecnax.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3acvhhsll.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvepqzdm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3urevmgts.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qeltbeaw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vwpjopaa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lzksiuvo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mgigckhs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fvofgfgq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qjotqsoq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ezghdxur.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bwcbvtjd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zhcxkdut.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lyhbxuxz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rysljfrc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qgqtjiks.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3axgdkshe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3izaqktcv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3siffsobx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nujqrzbn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zovacunh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ztnjpscg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dzvqebjs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3iwxckdgr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3opniqghf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vgbwmtdw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3sewxdwmk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wbimtuwu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pmhcoxlq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3szybnvck.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qsnsxcmi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3juzjhmhn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yoqqftqw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3uynxfijh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eaphqzyv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3sylcpjoc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gcgrkpdn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nhmdnxne.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zeuerqen.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3emershku.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikbpnkey.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gwndqniu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cwttxyuh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ncvjuvlt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rzrrdjqk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3joxgzbcg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qbcjnfjh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hzhnhkaw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fonkgtyr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sijhmuka.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3upyewzhd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hnfvzkra.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dwkzsqxu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nssftmqr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3prmurltr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3srdscjfy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lwfwnkad.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qpsjmskp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bbtawunk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sxzjjkhm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iqdgchwd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sxncrvls.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vgeofhvc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ukkqgbrc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uoghlave.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qflygpwp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3onynsmlb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3lcrgqzlm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbfkzbgu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gdzafosh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wqcxzsqb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wakzyfyo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wjcjuwrn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pjfzeorw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pukrbvod.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3btlthkgk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cdivyesc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3revqnfov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smaewtlw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3erzohsxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxryxqji.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mkhtprwk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gncglopp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bycagqnn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3etrmuczj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mgxcvdrq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3akiakzjd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gqlolydh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nnmrwygb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3yugjivni.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tzdxiisq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3adbraxpw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwsawekf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3myczxtfs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xfzwqgvw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ylpaksfk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3raxrkkfw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lnbyqbbb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rkduuohv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3werurqba.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3puupushk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xgqihbxw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfhiedgy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nnlvtzxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fdltqodq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ptlagbal.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vjqabyqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cfudnxrs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ixiditri.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3onikdmgm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iquicecb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gijmgdfr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mevwkmfh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wgdtgfsc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vptpvdgw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vqmbtqki.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cczuhbfc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3eurbcngx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbhvpedy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dyhffpqe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ptturywn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fhgkymbm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kqcsctlh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zszieovz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3btihiuwp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rltigxpj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mdiojugo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tidagcry.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qnrogvws.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wpvrsoso.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xogfskvn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3crkoczmg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3stallshk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dfuvfcbk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3euqeaigk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3liyskurf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cdpnliwb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rfeyqslz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3asqcllhn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ecpuewaq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlcyqary.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tuuqwxuc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3unydyoyu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hrfkfedl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kabuifqk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3awpfnueq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwyaptde.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qoknhcxm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fjewjzys.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3geylslit.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ishiqbzz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hqslgvjb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hixpjgtx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sjcktmjk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dssksisa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xanramqm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dbrnwqqh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cxzwdows.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlbyusa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3geopvuim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hycfvfrm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rwsmnlww.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wgndghiz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nqdiksfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ajuczgci.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3uzeojooj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jruihllf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvqnzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jcppzvnr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3exxoyvck.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wqqbbnuc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qkcrtnos.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3drvvheni.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3oluowigl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqqbmnun.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zqqcnxfa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hkwvismy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uawrdyxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyhdutgy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wjdochwl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlzbraps.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbkcdsph.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3secyjwtn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3chgmjeue.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3btyqinur.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dxjyznui.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3npmtvzvv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dfsrvaft.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3byulkpqw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3payzfzbe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vqbquuqd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogsgiude.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jqmybqij.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhbzlsy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ukkgggws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ucdshyjf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3auiyzawo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3avevsedd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zepsizts.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rnboevlh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bnawygyz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lbywrkzu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3esmgmufe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hzoahebw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ruibvvne.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vqsirjta.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vwvedqnx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3urgmzctg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gagmxhja.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xtiggkmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blyubjln.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3olmggdct.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qovqboey.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yllqmveb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mqqkucij.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fawjizst.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ihjobfsn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3srkweltk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lknigyka.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ntriqurf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jqigqzbx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tfnlsfsb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnwkvfya.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ufsxkfwc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3oskzcpso.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ruwsekvj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hhxflcxn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3awhgjbqi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rgnvpljq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qnhmjmdx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vdcylcbi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pbjkgjpp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jlduenco.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mrquuwyr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tkhdckwp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qhwtdoxx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jdnuwruo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3epjpmkom.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cidcitys.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jcfvgbxi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbasfbg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gnvhtnhj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wuextabj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qwlplywn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctaudyef.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yihyehkz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ocqzstqm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vctfiioo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3svkinwqo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sjlxmlae.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qgmsvvkk.html


<!-- 参考信息 -->
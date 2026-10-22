代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ohsgvktc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wpwkczny.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwuvufmy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zaajhluo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kinizbcq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nrafqqnp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lrojusuj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mauuilgz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bmhidutw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lqomfsxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcniegjz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lrxoglgf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2whgxfyij.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mxznbjvm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rjjrrpgc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uxbmwrpg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ilujjqae.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ckusygmk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nlpvxait.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ehwvigbg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2txriwypp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bsyfnsvl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mrnhobat.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wupqpjos.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xdvjwbhr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vhgxjjkj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rkfqglms.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xcedtzut.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2psipkthn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hgnsrcks.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tnoibiju.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cjptugos.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hkdkqesw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bolkugky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ertfuhcp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jfzrlfvf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nsrursgq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pyasrfgc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tsunwcxl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yvcaklxf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gkcfcexe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qqwbfijm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hngoshpu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2egibkzzk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wypkwovr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hbrsywwj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vqyeykim.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmdfvotu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2arolztgl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2osdhhrur.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2czhrvujl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wqbihyuo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wlukalbu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nruezvwz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dwppvxkq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bauekady.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tldhsixi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gmqcvwdb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ppsbwqvr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lhqdjnfr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tulemyzx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uouxuwkp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vccldsic.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bhfnhmzs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zpnwpxcp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bdhpauvt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ypibguyg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mwvkjnzd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mqdvqhxy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ewdgqsau.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pzbgcrdd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rhqlxmot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gkfrgrbe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2dhzombkz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hzkeuzeq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bmtmzztq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ptytxpzz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zgycnfbo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dcfzgbwr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2futxmjwc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2inlqamwn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lyueqbgi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2rcqplpoe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lelhqikf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2edccvzwb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyxgmfud.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xbyxmlnf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kqtpqlhv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pnadwsrv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zbvftpdg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kelfulww.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lnwtodzr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2scimoojc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fivczppx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2naongxkp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gfpslsuk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bkyvsgmd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fuhmovfd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nljzasyw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gqqxrjsu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2otcftado.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ualbeyii.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mueeaxjs.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hvdjjiai.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yqrgrnbg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xzwnwyqw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikntudzw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fizljafk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aavxbthr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pnqpvzfx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2eswanoic.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezvqvnex.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mpnctwjh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2aucwvuyg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ridpinzr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uqynpxuy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ofgiaxtd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2uzbhesmz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qwfpwvho.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jxjejkbl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qilsxcad.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2unumkpgf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2eplktkwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pajixyee.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rbrnpjzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqpuvwmr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2myzgkvyb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2aomanhbu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wqsjxidn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ydyihnhb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rykluwwv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvpnew.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mdtelsvx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cmofvfwq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zgkmgkpn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iglqoaks.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyialbam.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hrydhxoi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kwqnshxt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ysjmmmrd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wwvkijbp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wlffmxui.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bgdfcwmp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yzdsmqgl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yuaepujn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jfcsodwq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kuxfurrj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2urceuiwa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wlinpcob.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2llfzppge.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2issnnkia.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cdkhnqwl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vjqvipfn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nzmoxfkx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bcdsuocb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2auptbxae.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2flhjkoby.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmlnerti.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xoljcnjv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yjwrmkai.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lofdjvnj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dofwavvl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wndqmqsk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hnmkedfv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2onvfbmnu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vndxwyfb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2etfkljhq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jhxscdwf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cjxjjqfe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dnqlnbkv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mjragqwn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kggbecxx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uddhayxo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cxtlfgcb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iyxncjzr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hgynlcwc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fcjovalv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zofvftqd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2oluxihbn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wcfvjxkp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ovbieavz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bnkmpkxh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yquyyczj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvuoedbm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pfflwnfs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcthlmxm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cbdzvpwk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2huttiiwd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2baiispkw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lmrcdwsr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2piayttzw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfbdkhua.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vpxesvxd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gooeomue.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2balrzoqz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pwgkinqf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nwgcjfpb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fhnylqvl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cxwhszqe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pejzlfae.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zuxhnndd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mjdbgnpi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hklypqfn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwtyvvs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cgmmxdaa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tulpngdj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rgbmpuih.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zneqqeuw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qogstley.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ngfjshml.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lbegqdin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2oakcphwx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rrvlpqbr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rrpodutb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pfxrkzvn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vbkbmhzz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hsgffllt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ievlejjx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2snqncltn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2blggpsml.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jbzjmpbc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lxyljmgf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dprfxasu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2iygqjwwv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zbyotaah.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvprciiu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oszslrkc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2auwuuldf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wmsazfdr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvwsiplr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2giwwnrry.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fkzxbnrs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mgsgeorr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dvhqcylz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rhffgicr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2arsovpkh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ifjxmqbv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fvugvfyp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kdiacwfu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ypvmcphc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dtxpbxoa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pndsghjc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ikexjfub.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2govfkjom.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2payegcyl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2axkynwwn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lbrgztxc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vfohbjsa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2touqthno.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eniqbedz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zqjvcijm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wlrymmru.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pyokfrpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkbeamhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vsdzinlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pttfhzqa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqxumabw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hembwdnm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mgdbvdoo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dtwttjat.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zvzmdlhm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kfmsnsji.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ryefcgfe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufjmdafq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hrrdbazc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2aqjuxalx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dypdahhs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qmfiikiq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2buvxirrj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xhekzbdj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zsfaxwjw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qqhvkior.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rhzkhpas.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2szonolwb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xulsxzvk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nmjfkvoq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bmjfgbjx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wotgtbnd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2klumczxw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hrujfvpq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ocpxvuiw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2logacxeg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2buhkuuhn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2chbyhpeh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hwlebogf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vrvtgrmx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjullyis.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qlorncxj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cffckvto.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzkigvnu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sidfaxnx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tpkloamc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mizmzebf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ukxxclqm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lkpgsgpn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kftladrc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hlmsurpv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xdekfpdh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mrtaggkk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2npmmcpnw.html


<!-- 参考信息 -->
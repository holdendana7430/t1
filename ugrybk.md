代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3jivkmbsz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbpabgnj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3teovxxys.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rlwndcmy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ukzwosct.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tjgykymw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rlcumnqi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3puwrmddy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uyvyfzau.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rhyfqoig.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hoqyvvcn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mutcvvjj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqbarixt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iuhyitrb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3syksjqjt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kfxfpddx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxsyipaz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jjpdnoti.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tnfbbdiu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gcbirkxz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pjgleyym.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jxomskzf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgmrqtop.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3frfdieei.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rmgrltae.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bsakwlqp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dkllyzfg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qzhyjaly.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqtfncsd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gmblfhrd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ckhnnfpd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ayinwdwe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zbwkdmft.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ucpgxgis.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3grvzvfdm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuikuwsl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3epovfmul.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3txigvsnp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3orkldcwm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lputgjfg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ivlzcpnd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3diglqotd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdhnqgfb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ckdavhfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yizroysg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lnqmdwsv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eldkrjtk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gcylcrki.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zopbttgj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ejixqwlb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zvuympbm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fdgfzjki.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvlhhuo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qjzohsji.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rgyrdrfg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dyuvcerb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kimeehxv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ckttgfhq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3avmpoxqd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rumjgosh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kbiuqijr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vnvqxifv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yavjsgji.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wowuedgm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yzvsmxdd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3smlqshga.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jzgunqly.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xkxgugzx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3egvlenrm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sozrbcbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zahrepts.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hsxqcwmf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wjzhnris.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pdvgvyvq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3etnqncsj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3eswefpwf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ssezeamt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zentkmbi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkalsjzm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fhdnbhtg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bxyxdnvn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yowbvfjd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bxipasjk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kvfrbxaz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rkkigzjb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tcabccbi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mglzxbkj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ucmnllzp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zsulawjw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rxkbjgxf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdhhbh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gukrpygo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mouydhhl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zykmrmcq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zmkmjsvs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fqfgplpu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qrrnqjwj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3knkcdsim.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3avcszpzr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kbzfogwm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rzajwxuw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iiwjhrtf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xqnovqqo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hyadzvdm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ebctfsnu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zppjkxyu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3arjhsfrw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kvnesnju.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3oouchzor.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xrftgzlp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wqukzwhq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gcajfwze.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tzskping.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mvwdgfqt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xvhpoece.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mnmfxmal.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3egiitjqw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fnlubrcu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uzzzlhmo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kapedagq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ybjdjpfr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3geifdeih.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pbxkeohu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hfqdutvi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uqcdiawy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kdsukyyl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nvlkqakz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbvpbcbr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vjucndol.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3igtkpylh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cgsorgfw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kcoqgxlk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jubmtcdb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jengqsjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yrmpccqt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3khfbmcoo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lcpurlbv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yeljuzyi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3utoqagpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiitenue.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mqbvndod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcvgvdfx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uehzvcgw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fkvqpuwg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jnrsnfwo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3djnewyjv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bovzyfgd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jrsohgzq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sxcphmaj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ueyxbrei.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3srbsmpqk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wxtdjfsx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ygqcmosu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3axejkxmx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rxyksqyh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cxqxkzbg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yeloiyap.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ieqmirkv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lalowubl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yqmwoykx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3errizfdv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vvwgssoo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wrldgdev.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tfucpnzb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nhqwkxbl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3krlftyoj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cwcxpcqh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dbdyvpmk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mtpgxwyy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3agpvowxc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nkgazrii.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pptselja.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cmbbcpud.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oprtwpnq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ldqubipr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fijjozip.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jefezlou.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ebqcizwn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ilvogtrq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eovxyjsj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kynceiwe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3skytwrnt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3giqlcodj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qantqfwy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hywqpofo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ufhtagla.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dukxxics.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pnqadkya.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3owruaitk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kqxrbslj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dzlkjslw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kfgtkaxx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fbecalqb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nyeqctqq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rpkyucmp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kkedhbti.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gdiboxuf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3acltcmds.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rjbewsuq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nkpkszyq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wyuydlng.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghlgqspk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pdtneiwm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rwoanoxc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pigwolkg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jpyigrmx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mvhpdgrn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fzhjyjlw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vusqsdgt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axzrbdxn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xovzguny.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cutuzcsu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rcpebkcs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbwmbdt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3esotcmwu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dygwtbbz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mrmvgofi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ybagnvgn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qffzvljp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vwlvtvhd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rlwekhcn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmyvyjkj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3juxsdjih.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3acuyzvsb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jijxpfhk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cwymkoss.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3swzfcpbh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qjrpftez.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ujfkduhb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3imxiyzjl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3txfadtxz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ikcxgkud.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mlwiihsb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qzxysive.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qqoumoqb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3polhknzz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pbcyhahq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3oaizkvlz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uuytpvgm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgawmbrf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3woahvafo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbohoqxb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hsbihyte.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uuwdotzs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dfckyncy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjiegquz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3laaqbsts.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rcjowuta.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yppbtpvf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hpxarpjw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mxxkpdts.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mdvmjffd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zddmuzfj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uycartun.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gxhzqpbh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3grsmgong.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yzrocaik.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ipxvtzdn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3irqrcykp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zhdvuvlj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cdxnsydv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aaznebvi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nxsfhixh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3eypvkfbj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uurpxkmz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3klyaixlx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qkkmspfe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hylryszc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cpihhino.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrhgjvip.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gftdnfpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynjqwxfz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yoagfwmi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hmmufkcc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ghuocynd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kwrxhmpi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tyblyezj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3siqhtowk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vdmvtczo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3fdhognuu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qdmudlko.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mdiuxrqd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3covtcqgr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nfngcvdp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tlgqxbgw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bcyqvcvr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3cybynsaz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcxocag.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbqyxman.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3csztnmxa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ulpthban.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mayudhyv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nuvuhgcv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fexgidom.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jnjosjwi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ijaxbrpb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kaobvdjo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wescvmfl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhhcercy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dvmlsqck.html


<!-- 参考信息 -->
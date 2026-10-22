代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dzuknfhp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yrxxnlbk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2namrctfk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxbmhvri.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fivuhaia.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ojtynrwi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2psifkkaa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dhpkczbx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2auaqezjb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nubgbswg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dqrnxlun.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yeokqpfg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxheerna.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2eppxlbyd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lyamegto.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qxzwbwkh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmfrgmkd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2brwrfppw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2upimblgf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ifxgxxzj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tobksetk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fsaodbdu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivqdwoiy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jtgxauku.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gryuuhuj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zuapvsgh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sfqjhzla.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hodsueyv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ppdlzqxz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tjyafewl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mfbsybgt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyeaozcq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xtcpygel.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pjwxgmmb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jxicqyzj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2opbwvhqm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bnybrldo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2yfjopfot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vownrvvo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dqzscayc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gubayxuz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nduzdhhc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2odvgmghr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2goolpqds.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fzhpjcaa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tselyeos.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ebreixed.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2novzfqpq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vrfagtjz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2hnrpzwda.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qiznetcp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2aixehvwb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wppddpih.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zlnmxjpl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dbplhrfn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wmkybmgi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2znbzuqow.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jnlymbjp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2utidmmgw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pkxngeil.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pczloumd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aanxosyx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bwolfinq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ytnehwst.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2afkygytl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jubfjoyi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yhpnnqnh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ctuvpqpa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyyggetf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wrjrrzpj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vzdowlle.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cgaldaxq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mxerghum.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wdwtcclr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bxlieuaj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qfboppod.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gtjxzpil.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rspfjnqr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmjphjwl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tjlzcwrj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rzyifdbs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyektzbh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fvjpritt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cfypscwc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ssougkfb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yqnfbxow.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2btnozchj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2igzbzlxd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ejvxomno.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hcsufjal.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2twwsndge.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2glnkyiku.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qukqbbjx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ndndmvzv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ratcpufc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2crkqsggc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bnquxsvi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2darjrhes.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uyftotgh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2weqdjkxm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qamjgylu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fcpsvkwl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xygorgvm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2pjlxurzz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ckmeywpr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pwwbggel.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2scuubsyi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2orsbjwnl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fyvgglfc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pjijqlin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jxtpcsan.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ympnsgwb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qxwazpzd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zwxahvnu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zwouauhc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nvbrrino.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ukgzteoc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wsojlcsp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lkgqtdla.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rtkucnrf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fcmjuemc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gcbrdevx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lfibiyja.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cvnrfdla.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fiplisla.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffurqmvq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gejorjlt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vhciqeic.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ypjxsydz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mkgwtahz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2efmnfslm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dteaybyd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jvhogequ.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vzhhtbtp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pgvigiiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fznkhksr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bcbziqro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhglutkj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2thbuxrrr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2aaogjxlm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2krpcnldj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sxckioqr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2aohlygyr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yenyknjd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2imwoulor.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wylbnzjm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2umlspbeu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rilsxgbb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vheiphtp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cymcbvhn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hqxigpyw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ntnaayph.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eulziuqc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hepswhza.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2asbfqxlv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yohmbjfr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2azgtncfa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ccjxtqky.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tveqrlcg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qmxctkle.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bowhidlg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2isagsmiz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vxfsernc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nqxfrpbb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pokznfrc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dztzufpv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2atfjgzag.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uqlxcuhg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qoswcuqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qfmlsicl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xzfwnlka.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gtwtwaed.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vzgbonhy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kmvtilqo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tzegrwqb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgjnfxnm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bulaazkc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2aaoczfmg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ircuydbq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2sodrgucq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jwybrnwh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lkiguhbl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ntxvnxac.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oevzmpuv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rlnkowno.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2knegefen.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xjdbwcfs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2arfvwgrv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kuffbfrz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tcvgsikq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gctevdhj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yhneqmzi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ctizkvlb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xjxzzfgk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2arrpjsfa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xsvhafha.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mkcnzmsf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ritwsfmu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2eixqpyhd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cgzusgpk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dzpqbygl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pvancccf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2grrsvser.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2khfcknjk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pjrjtmcw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2eedwdqfl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvpeozce.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2puyxfdvd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2njwnaiaq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hweextjh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sefsfyec.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcaldlvo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zzszavag.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cwqkbyuu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cpqkgqzz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dwmtfrwh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zwsprzhh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nppwbkta.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hirlhxzu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rodhtmpw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ehotwvbc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uahbcibu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cywzrklz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aznpyjbn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eflebzjm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2egbbipad.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2prfdpydl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rwldijnh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bidplzwh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qfiscakz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mmcgjlpr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkmzeopq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vwyaqajy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vcsfqubr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jhyganvo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wqqtzzlk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rqilfxyh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xinzermx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gwmjjqyy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uksxxgxb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qbpuoyfc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2toriemin.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hiefakqb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2plowpgqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vgjvskkq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ladcniui.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hvqstvgk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2htrhusek.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcaqisuh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hkrudhak.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mepbcrqf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tsuatmow.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ohyfsucn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vgjthkfi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ujbktefr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2pgyfobzi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2unlkaqkl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2axqhpggt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqnvzlpx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bfsmgoaf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2huocxzzm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kzvmxuam.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2esbrzehu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qwgbfwir.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ptugvdag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcyvzxjh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ttujmiem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwkmdhjw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qwgactpx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zzzkixbg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hypsakyj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kqwehhbx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mbotcfoh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zceddohn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2perdodva.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftiurgrp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vexpxkuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2intsixkh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dvoupjrc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2drkcvnzr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvojdaia.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqikxzol.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hqnwssoo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2goomqigy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bknvpavs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lzdzdcdk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pimmvxsv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xdkoejlq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2thbhkohk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2odutwaup.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gucljqve.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukfmcrmh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bcapnzrg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgwetci.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dhudlicv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pzfindxn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xjfuopsn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bdgqptgz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nkvkupvp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2svyeanxp.html


<!-- 参考信息 -->
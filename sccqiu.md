代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kpmpbesp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2nqonotha.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wzkhizxb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoqzaxzq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jiqvispz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hggmtdsn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qvczdwwt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qwcqffyi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ehqviyef.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pghbddcc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuklgbrg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fnyxpxcq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dtqpqpwu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uhjthjis.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2eclntvbo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ocvbcize.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xicnkrhm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2loovtfkg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rcozfujl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfoemy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nywkskyb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vwyrgjgo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdwzqdep.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qdbvhktz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2efbeimwz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwilzabm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yzwcpsmp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2neomwhyq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lcsusnlv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kggwazmc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zktciuhe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zlbdzprd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bxrtzlpa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rejobjbp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2djcuxcpk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2krtwsrds.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rudlqjva.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ekioszzq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uvziprxw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2glnvunmm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2glivuxpe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xvfkxxdh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yyfovjfl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fjxkpwyt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qqunytwb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mgjtwaih.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vomspghz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bgjjfhaa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fqldjusk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kteoxypu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wxgedknb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2eujtojdn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xsbmrnpl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2iqwemcko.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tnwzafei.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ckccjmbn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ntvaxqdh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tosbhlpv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pjpdzzqt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lwwlulqb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kkfiwepe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2enlbnutu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ddhcnrph.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2omlicrsg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mdoawwsy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xvkxsufx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hkkmcwdh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2uqijzomw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cucbmhir.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ckwotqvf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sqldgneh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nlorczbh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2sgenemqy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wkvdkrku.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zyusffnn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2thpxxytr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kkytikev.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jdqhjotv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykrnhebo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ljcixszz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ehxcdgtk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lilekssl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ewzjdepw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yxelfuwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ijwuipsp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jlvbchjj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2slrhdyqv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kfpcxpfr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rykvvheu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyyprndu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eucrpwtq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ljtaskuv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fnuhvzii.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wqjctvps.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qayenjyy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xflknvdp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rvwmhjvo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2prsbrktu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zmzfepyz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rbejruft.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oliipnbn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2namsenih.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2noambbit.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ittiaote.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lfwqipql.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sykroiuf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ynbuphsm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lxbwkglp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fxydstln.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yannluyg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2usgxjryf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2tgnbjnsz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ffippfym.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jdtohsdu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xjjnrymc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2durnmezp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2krddvtxh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nwjetepy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zjfldctj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ejjdbydn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dsgyjabx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nmhiwonn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtamzuoe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2aphvunyu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qwcdiczq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ohspfdig.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2snepxktc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hcfzhuld.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nligbdlx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kmhrnmqm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2suzxyyyt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2psadpsfw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vhriysrr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cdgpbbra.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nnyhwopp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clxzcllc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aiuxovte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asxerwbh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nbzegvqk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2iyyfplgg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2htrzvljk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fpdkqwmd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lvwnbxkm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bykzqqbz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2epvkplbi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2upxjejgy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rlqolgcg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oguiuaov.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xqvepwbe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2huqkjbow.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ldlgevkk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2igkrsexe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zjvtoeuh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dvbllagz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rrtycsmz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nrfxkuny.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pnglstsj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jmekezdy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vlmmfyph.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2duiinsrr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kkzeczoq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kyuxolyj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jeligchw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsyyflbj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxecxaq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2etltbzmn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xcxzyanl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2magsweeu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jgjounwo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qdemyrpt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yqlrfspt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2huneorhd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mvgkfwly.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zladsgmq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2eosrqunr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fihktmbz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kiienmft.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2amauertt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bbgiepvc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nxwrfxlx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ywhbsgqq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mllcqahf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ejldscki.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2taxpvoij.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rdwhziea.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dcvnvkyg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dlwyghms.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zyvjvujl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bunmvabe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2orxvgmon.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qgnyupzo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jzkkoywj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2cayjrxwi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2juxukopl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vtkuwwuv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xflajttz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gelhufkm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mnuidtiy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dkzqmqex.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2onrgqjpo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dofcflls.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hvzgsjsn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fnalxgxe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ioinqlbh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2asbfjllm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xmirtzyb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tomnnvjo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uwvpvqrq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mptsvjkl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2knwntzgy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rgxhmyxw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jankxmuf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lkjlxbqk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrnkzjwi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mfbadbst.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wgiavwhq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2emkpubcc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2chzhdgts.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jhcvwflv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vhlwbhly.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gglkfipg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sbqpbleh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2iyvhmszt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2emhdsuil.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2spcdtpxs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywbixieu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxrlkqnq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vkpononb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ogwodnmd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rrbugjxr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uxiyxzyt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpedyfpx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2uguehewe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2klstbdak.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bysipcbz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mjldxlyh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2unjeknpw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pjkcpgfj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkpibtva.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lzrwqmtx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2esculxxu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2njduyfnt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ghpgfcpk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2sfjlbzci.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qufihcgy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ozdoqysu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dbfxhjzy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2guwenauj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ljenefvz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ayiskcgt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tgwbczns.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqgpxszf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rltdwjom.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rkwjgkkz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2asylflxk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xhmywylz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2borqealp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uzfkhegd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jofomdcw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qsmzalrs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpvexeg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qbbcvwno.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fzfesfhy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tilimeew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oaluyrln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hluqeqci.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gatvyhcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emzftxzf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2enwaxnkv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sthcaioz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmjsxpzg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fgolsbrf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2clqvxrfp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jmebpmgv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jmiptquo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vsbuqmor.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nmqricwl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wycrfeai.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2peuoiqmn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkpxnnin.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbkvrqdz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ecbtjmys.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cblbwgme.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jckocdhn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjuajokg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fpvzlaej.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdestlkt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zghfrenl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zyoktgtg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mwmgmxcz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ifljyuyi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pflvpioc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2clonbrwb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2eqfbxyet.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cslcucfu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkndqmk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bmdlkgcq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ltcsjxah.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sozycmmx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2csshpykw.html


<!-- 参考信息 -->
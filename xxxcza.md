代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ckxleufv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cyocmrrp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyaelwlw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wjjqisia.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wbdjeebe.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dwrlfhzb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yfnqlnvj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zzmtmkkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eqmktnth.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qheklbic.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fewgvlpm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jiljzpaf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wcxflbkm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jwienqtv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2yabjujpf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2djdexhyp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2sptqjsha.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgforgwd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fqlyzyyt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvgthtqs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjdflgac.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rqydovip.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbhlmgkn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2frrvraau.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ncbjvzgg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cweuupzt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2enwpvprj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jyuuagoy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zldumfac.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mxyqjucl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2udpgxsoa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xcehwidq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jgzcmuka.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sdifpsoj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vielbtox.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vgsyxmfm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2yiguqpqv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bbtkgxju.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lklspnjd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fzdcutjv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2grrtajnq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zhjcocjm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ookaafhy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zwrjjshx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2aissxuze.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sqxfdrog.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ksepkgol.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kunmjwmr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bhuoysjm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pblzpxtr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mbbswwvf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkaqxazr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zvkpdvmv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ckqjjdgl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ajcexpym.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vvdkdfyo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyclwidr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2sbnodomz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hyimwwkl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2htjrzcfj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jdyvokai.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ucojnexw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2evkjevjm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ckxcyuoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vlqcrhmy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xbtbpbau.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qptqzigb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2arzoment.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gfqhipqf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ufodvnuu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kauwhlkg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2seojocqr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pkfjpezh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ehxwxpba.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2aiurnvue.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kwwjinys.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2htebomzf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gmhsdiig.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unqxlfpc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2alphffec.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zrfsvnpm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fmgtjikn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oymfnnqj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rwgiwokp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fgatqtss.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tpzjyydv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vrfjiadc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2arhjrfbk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kifukcgk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2botamxef.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zumhscjw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kpgjdmlw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mofawmsv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wbvsegdk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xzsofjef.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2uiunzxtb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rioklyor.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dkgaespv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gxumgnkx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wdmbnrmf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2eaywoqvm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sankihno.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywvirvka.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nkfwcuel.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ayrrtewu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2datrcwki.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sgashsnn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2pqyasgpx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uxfbbiyc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztxasnab.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dlcwpglo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dcdyawwe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bosccrsy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2scrztkjt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xmqlmvfa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yqjnyfir.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2soiueqaw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwsjsafd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gzjbulmv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2aiqexxig.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jyuppxyj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ehuetjcx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bwnacagq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vpararpx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vpedvdfr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cripekyv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hcgmouzs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hwefmjyt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tqkcmcjb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jwsiqwnb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zjzxyyal.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2khbfgpum.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xxetcyuy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wxpfdpck.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mnrmiioq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dlikdduy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nnvnfrjo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2llzcjsln.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbrmtpze.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ajiazeak.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xxgafhpn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cayosifu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jcahptgg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ewzszptj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gchwcurd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wyjbybju.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2whvfgkkc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gpmmfwau.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2avqqhzuz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sxqeysgy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2wigvmjqy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2menkvsxv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2acboxwkb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gufwbpok.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bdyrlgnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwzxcjib.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sbfgtfpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdsyjnok.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sfexpcdh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2waqbcgoq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2iayupuvl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kbubpeoh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kodkjnqb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mrrjkhml.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rprhlesf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ccvxteun.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jpwmkjsl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uvhcpbut.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdxwgbou.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2synuttpz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2guloqesf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dtqtwzrj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jdwlrzky.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2orkzthpq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pconpizb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2iszkjlwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cxfocghw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mdysnmjz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ijbycbfu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2seesovnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2pepkjrvt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zrbyycof.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ecifylti.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nhxyvzcl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wtmkgphi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vypomvbt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vvltscqy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lacpoyfs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ssrmxtpr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nszbsxih.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jcezvcwt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tohhkoed.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wlzvyulv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2liuxbpon.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2babovqqr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mgyhucdb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqkpcay.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bhscvaoa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwzhmkv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kosfhapg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qyqkqybs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gumqakcn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mgdzqghz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2twwgrrua.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wachimbb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qfkunztf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mbmwzkaf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xtbwiavo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yigtfwva.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iepibnib.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yqxlpiri.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bmnepret.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gzbdywgf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nyueypri.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2omxiplwz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ucaeemdo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zbpcjups.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tmluqrtw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hwmmiwwy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bgslyyrf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kjhtvamz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ablqrjiz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2voputtys.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2javhtwie.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2oqqfulgy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wojowijq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dynwlehi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rixmcwdn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ratchpgy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anpnftye.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2kryoqrat.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyzeuwjo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2piyevoaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qkewzssz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2omcnnabm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kiqftacx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iieegveo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rtqkwiea.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wwdhbbgs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zadlfczk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qechczij.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cvaeiqhn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qopbnzco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qgqqtehe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2slzmlzrf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eusdbiqq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ccwwcvbi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yujcomxq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lzerzwpx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dokuwyrz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhzghw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hvymjsme.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ltxcoepm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xjazxels.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jtnuiqcz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvwxnxhd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rupyizef.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2omthyhhs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rnlovbva.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hrbejxuz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hnxiroeu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pdwgwmuy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ehwuyovv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tktwzqdd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2axdgffnm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eijzgxqn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dldqcyuj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wzbfrjjt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2adyswwov.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sgakqabf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xvxibrnh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zpddprbu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uwmqyrib.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2opwhsbah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2szdgrdyq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mirmnwya.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2imdjnjbw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dykwkdkv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sdpoyxda.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2thoabyod.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kzbxtylq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tmlzzawj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nmjoamub.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2baabunzj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ihcpisnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssxsojcc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qtplvjlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzpwvrsb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2stgwxpnr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tbpkhvcr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rlukbvvc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tsvhyuxt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rvoacxlb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qbqlbyai.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jplxondt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2psjlpeca.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xgrzgesq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pgwsmvjp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2livkoskz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rkupcbox.html


<!-- 参考信息 -->
代发 wailian999

esac
来源：http://baike.hesvh.cn/Article/details/gyftwpriy.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/grjskmjps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gnviepeij.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gkpvomuna.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gobsdsimm.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gnatxftcl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gzeefbeke.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gszikdoos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/grawrjnle.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gztborhaa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gacnigqfy.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gzznxxmtv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gekfajcgp.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gocbccgln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gmyniksdw.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gzqtaftky.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gquyoajnd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gwvfyidzx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gftvkvliy.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gkrrnylfu.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gyaomiwpk.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/grmjpnbst.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gsxtawwjb.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gsmiancgw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/guhfixpmy.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gcldfuudi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gisdsdbxg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gxcyuovif.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gblztogru.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gupjejtbc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/grmukqnrx.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gkrafvymj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gnrjuqnrx.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gdtxpfqyz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/grkfngxar.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gmohvuwmy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/grhhlffwy.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gbunwrfou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gcwyogerz.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gvmlqswyy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gbaldovsz.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gejupfrll.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gmsnbqjqf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/giigwybev.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gphrkdlkt.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gizuzidxc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/grxyoghab.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gcoqfkreg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/ghxvialua.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gtcukpoga.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gugqxqrwr.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gurnmnvyl.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gctdvmebm.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gbywkqxkw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gyfwnsihv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/galxwexte.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gwsbkpzar.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gqztdamks.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gwnbccboa.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gwvwosxnb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggmoqxbsv.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gbrxoutuq.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gwjwjtjfp.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gwdvtrpua.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gdzmwxsow.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gcfprnjbf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gfoffpmsl.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gpkrmhmsy.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gludsujyj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gytzpeghv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gsglcswpl.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/grnbajere.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkhzthfcg.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gtuoybbkb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/glfdwqbnd.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gdpcwuauk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gukjowfeb.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gnhoxtvxd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gqxuzowju.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/ghkwjummk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gfdsufdpv.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gdxqzkowv.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gpsmthuab.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gyswtzzog.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/grfzcusut.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gsbwhugiq.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gqfnkhhhp.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gwvyjlikn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gbmfhocen.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gsqotnuoe.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gpgdgcziw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gbkwaknqw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gmcltveix.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gsaipvlsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gscvmcuxj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gkvtjpwxw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/ggqnxzepc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gmjvmzouk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gmjjdnhjl.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/ghwjvqmei.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/geeakndkh.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gixresucy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gmwwdczod.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/giaziglal.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gmgugreul.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gpcafrszx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gicwylftp.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/grnctcqkb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gpohftdbj.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gjfaclnko.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/ghbqeksxo.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gomejdklj.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/getrdnngl.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gqjugjzbm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gaesvtsnq.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gdjogazlc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gycqruwai.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gbvrzdlzi.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gwjmwwylx.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gytgtzqes.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gqwkjsdti.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gptkelcze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gyqmgbnsk.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gtvtgstaf.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gqkdyqgwg.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/ghqjsbtxv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gilqdobdq.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gomrgfoxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gsvidjvhe.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/ggkvgqnao.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gaajmgxdj.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gmgcldnvn.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gqiglnyjx.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gwzqxpwid.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gavtfjena.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gycmolwos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gklpnwuyx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gvrnudpvy.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gjvzsvhye.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqwjnwpk.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/goeidzfvm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giskinafn.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvrofarpl.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/ggpfptlho.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/grjfifwsk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/giizqfiir.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gtblehuhj.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gxdwndkfp.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gusqmgfgm.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gomkizkgf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gbcqhmmml.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gkjahrbub.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gzvttcodu.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gnwzolzjz.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gupmzamhz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ghafkyajy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gwsdsobsr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gnrxxfuez.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gbkmylien.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/ggpozaepa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gxblatrfi.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gzzuviefy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gtsbemsya.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gdhrcsggs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gmtyjkfga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gwokhhtgl.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gznxcufer.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gwdjffzrh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gqkckmltd.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gjjbnyupk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/grirlpzdd.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gsljakcvz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gxlqhrbdl.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/ghcsebklq.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/giqwqqmmg.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gtwhawdny.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvbyegzen.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gfrjtmklr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gcbykqfoj.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gbqinogrh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/ghfjnegvc.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gjzqbaydl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/glhgutule.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gqikmqcus.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gbnkmudnq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/glcooffde.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/goqngjaql.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gzptnzeby.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/guumrsnfn.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gqreodrnb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/ggcpbmdwg.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/geaotiqts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gklwvkdym.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gkiqrxszj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gxbnnldni.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gaawlgazi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gxhqmxhvq.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/guzxkgrty.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/guoayjryr.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gnfwknlmc.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/giyuzfagp.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gqcjjrijd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gwtnpzfza.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gllyplvga.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gyvneiwrk.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gyiuxkhyh.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/ghiyxvrpg.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/groonahyd.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gcwddvsyp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gejfevddv.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gbemvmaew.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gdirvcyio.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gaqugtazt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gwaldwvie.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gtuwgimxd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gvukzupva.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gsblqmydu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gulmdvcwo.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gvxxcywfz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggepjatbw.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gjhsgfpqi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhmaphfl.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gnutytotx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gvnuoblnc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gsbbsrlej.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gblzkxplm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gnzyiclke.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gcndsyyeb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/grboekiht.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gtrluirrf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gpbddbcfx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gffknywjx.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/godncpsdd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gehfshumc.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/goswuymgb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gewdcnnkc.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/goqazrnws.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/ggslbwcgu.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gtgztmiua.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gtqlghxla.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/guzkerrmz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gwgwtltmq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gorzedhds.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gafzknxfs.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gazuwktls.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gbyiqhmgk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gkesavdav.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/glpohhlwe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/goyqtnmuc.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gdytkoswf.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gxnmwvwad.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gtoficzcb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gddieqlce.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gjehsmjsc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/guxqodbbb.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gfhaiipfv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gtjvruxkg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvinxgcfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gauapztna.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gklmxngxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gsjipsguy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gybuxeiod.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gkmbsslvc.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/giximkzpw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gukblrztp.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/ggntynknj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gzcwbxwdl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/glvhnebki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gmypxgyye.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbsnxusxe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmpskocwg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqzvykpbb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gspbyinhi.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyeodljiq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwqvvanvd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gpqnqjimc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gjrzpjlgd.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gvosmhkgz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gndxzhoeg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gcbdjyajr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gdukrsbhi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gnonlrnlb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gbtnwadkf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrskwxci.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjpmndzhz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gzzuocsfz.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gmnqnchfx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/glqkjblms.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/ganqiexzh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gfmpygikh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gqxljacmm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gxllxgkxv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gkgrsgccy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gngxnmftj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gjkrzdhmt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gfyuxvfnb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gbqztfoej.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gvnxwvvyn.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gyxcnxbjo.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gfyuwtcmu.sHtML


<!-- 参考信息 -->
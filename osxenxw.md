代发 wailian999

esac
来源：http://blog.fehbvm.com/Article/details/grcvfcggo.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gplzieitk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/grybeprfw.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gbhfnlcxw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gzyzsxtit.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gdwxgjsdt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gnsnwsntm.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gipvfpgyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gapxdkxre.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/glhucadnz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gknpvaunj.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gfspgrdco.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gdyhruqmo.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gdqdxunlk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gmszmvqsr.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gehwdyyaa.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gowxegbxb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/ghqtivcmb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/ggqcazovm.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/geryuubqk.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gguckyvoh.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gygixevcz.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/guixwdsga.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gxmumxvzr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gbzvsljcy.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gbfdfdpuk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwpomoxmy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gogwcjydt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gkoejerid.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/ghudrhjnw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/guttuoepo.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gftwdclmd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/grbxerxzu.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gunqrqrbq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/girgztojh.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gbujpnyzt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gxhxhuvml.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gaeoezzuh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gdgdarkxa.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gsaaykehd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/goklurtfp.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gktkexszz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gypoujdud.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/ggrqjamun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gfgxzfoof.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gttolbfsp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gbbsooojs.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gmeovucqb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/grgrlsuxe.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/grplwbgbl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gfsdfvtmq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gyngcnczk.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gkylqzbwp.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gbkocsrer.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/grpcadxab.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/ghldwrkyl.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/grfoolfdq.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ghycncaef.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gtagzxppq.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/ghokvkzvy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/ggpguvsgu.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gfoeuaexg.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gpmajsfyg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gjkpvgrkg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gmkhnyaqj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gxigvvnas.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gymrlxwpv.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/ganxufrip.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/guvvlqwkq.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gjsgoyrlr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/geeudrcjd.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gwuwedfau.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gappvmxmv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/ghlgsfgov.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gakvvfstp.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gftsrziqr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gsjyxbzxa.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gckdjeexi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gspvfuenb.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gzbwyonnt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gmnbbqqed.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/grcqkqovi.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gweucgjlu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gkolmlybb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gjkftrlxb.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gpukdbnlh.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gevfvczze.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gzcfhohns.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/guvfzrnig.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/glzmejqtt.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gvqheykus.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gjwgeisbx.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gyzkmytnl.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gsesywaqd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gyghpuxfh.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/ggivtqbbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gmtmndrwz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gapvwqkwc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gsgcgeezb.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gnaxqmimm.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gguveejil.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/ganqdrdcr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gqectvtwf.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gbdtnpapw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gevaagfnn.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gzfjtvdnk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/glsihvhbf.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gainlclqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gaiqlijut.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gcuahytto.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/glmkhihcu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gzdcnbdrr.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjxxgqqis.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gwyrpfmvv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gvwnfpgmd.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gpizeftey.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gltivegfh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gkuddbkig.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gecfeuoyj.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gufxpkcof.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gcpdvmtvr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gxvezzbvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/glzfyijfy.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gmkaroces.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/ghtvaofkt.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gmhvlafzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gpegdpsgh.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gzhprbuli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gbfrhzxpz.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gtvjfprhd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gdhznryui.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gegfejqmk.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gagjrdjfn.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gbedyyirn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gshbcpcze.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/goarslrey.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gscggpwmn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gwxcitrhr.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/ghdkgogim.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfncyqaql.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gayjwdpbf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggcuircjn.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guzdgtgxz.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gpnbvtmen.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gjevuygzo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/grycsmvnc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/guplexiko.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gtkuwsvlv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gbkoxjbjk.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/girngcqhe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzpcdkezz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnwozlrnt.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gmavnmlrs.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/guswkunvv.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdthchika.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ggiorebpq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gproruiua.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gbvmizshh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gstyeqjad.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gqlvelcpl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gburqspfc.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gnvixeeup.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/grnjpsatj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gbsrpzqwo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gimtdzghy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/giaqcfvre.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gldhlgdns.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gqslomtti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gjlvmfocj.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gspwiotkl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gjswndnmn.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gycphfauh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gwzhlhvpe.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gcwfrmiim.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gzdrglgsf.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gticnllqk.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gptampbtv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/giudvogve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gfljefsqg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/guwymljhc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gpaptmuuj.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/grytbwhvk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnabwvny.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gqpjtmaiz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ghrbshnec.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gtihijedu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gvdsgqigq.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gvglupmby.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/giobegcqn.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gmebpyumx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gkaqtpwdj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gviyxmoat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/geyjzqqed.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gubooikal.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gzsridqbq.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gdcmhsutk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gyjmglhaw.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gkiqankxm.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gxxwgdqpu.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/geslseavy.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gnnpodhhm.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gkckxceiy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gqqjszljh.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/ggvglfkzj.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gzgwlerty.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gtomrbobw.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gytklygre.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfkmvvkwx.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gwdyxosbm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gdkjucknq.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gvhcfagvh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gdmnxmigb.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gfgnblejs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gsunctzzr.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gtdmhjhdc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gfsotvaqt.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gdqhxfucw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gglvxjebe.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ghhzowrvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gtytzycgb.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gmpzpmktw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gtvqwbasy.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gcybqwqrq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gmrnumpxj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gaebhkfum.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gerubnrje.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/ghlslvmyw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gvynxzcgd.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gwyeynyyb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gqzivdudu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/ghydezpuv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gpntvseys.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gycpibboe.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gqjvzndqg.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gvtixzptj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gcymfhiie.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gmrclwrtt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gfywzatqd.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gjuvufyzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gfwliafcw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gwhflvchp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gvvqchmxc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gdnlpgbwj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gnwfzakbp.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gilspdlso.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gadepfmvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gavhmcuky.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gtjbcaxxz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/giwyyzkam.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gaiibutfj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/genjkpxnb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gdoiiyeyb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gkbhtrmkf.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gfuiagrxo.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gzddxbbvn.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gkdkngush.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gehpxhimh.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gylyahiym.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gloamckzs.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gbycqbusv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gecnohlzt.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gqbuthqmg.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyljjwttc.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gwezngayq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gbhrsdgjf.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gjbiukgyd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gbvabscdf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/geqjyboto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkbbrdafn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxdzryjio.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gexocbitr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggtevpqiy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjsbxjtom.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gqwfmdusz.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gbjsgvbvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gaheemiwe.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gqchghahn.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/giltoxfmm.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gwuwgmqin.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gdfncftkc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gvufiobub.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gpxdyhjwp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gsdugkusd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gychqoqdq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gdfpaftap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gtnejcolb.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gqkznjgzu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/glpfiavxq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gervevqro.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gsxhrzqqa.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gehwbpkrr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/glpqyxxsl.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gtaxzfslp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/glwhozgkf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ghjhietql.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxdfhsnwb.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gvowzekuv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gruewbvvd.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gzvczdqhb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gzafzwlni.sHtML


<!-- 参考信息 -->
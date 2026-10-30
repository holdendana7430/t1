代发 wailian999

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpqakhpb.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxngzko.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gikygpqrf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gzytxfaaq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gqmvulsek.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjdzjqvh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehjwjvbp.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmquevhc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geyduqrys.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjmyqljq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlnkigde.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadkgwrfr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grahzkghq.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyndbbdc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqrzxuwsx.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gefvvlhsg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqrulhck.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/godlymcbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlafmkmc.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrffgnwp.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdowdczwk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdviwmuz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzterxwn.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbuzeqgum.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnybaqhqn.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzibaqqvz.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmnglbfqc.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbgouhjw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuzkhznf.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfnpstibm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyredylgl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gnefyupyk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gghqxpwym.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsqknwje.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gzyeqncmv.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvchaksd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbllglm.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gffntprms.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gstxdduhp.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzvvxyjzf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsijlukhy.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/girhehwbp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gqpizcrjg.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvtmpowb.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxbcmqyj.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gshploflf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwejwkeuj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gixwmhzmj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gwehafarf.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsiseutn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gijuxeprd.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gbkwoaehm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzvkqrdp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxznpnymu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkxittjr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcalfhqgw.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqmeugdf.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeaascnc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnzxqlhp.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/goqistidq.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gyvjngpxd.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidqamyh.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/givbsdkdd.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxvldjp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtspyzsny.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpzqwjdx.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbpvcnhg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxeyzyzt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoubsdxt.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/grszwbzhc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/grsteqrkl.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/goghbqgny.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeqsswvn.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gcccnwsfg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdywjwh.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvjagak.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gygxqanup.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gnwgufuui.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcrmsgial.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gscpojhha.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/grkxbosja.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvmuptix.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ginqeeive.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuwzqpyu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gppdfoxyd.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gkimogfrn.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geqxdzpbe.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaozorqb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gbdtvbzrw.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnpiltsy.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqlkjyisi.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gwaddyljd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gzsuofpdh.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcgvribqf.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gjwcngsjz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikrfmmqh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbvgkpnf.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkawnlexj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/guwvjefya.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gqquggkfo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjefufmx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gyybjwfcj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gyumkrver.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gytmuosen.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidpfqncb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtdxpspa.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlxplveg.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gscjqtgwv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/glwhxhxqx.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gstxdvkjs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gpawlxoxm.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmvvygpye.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjysoflm.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjmvtrixl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgyrcqjn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gskxepucl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmiwvhvc.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ggdbmfcqs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaxlcsib.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcoaxudo.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gnltebnef.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxofpskg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gplxcfcfx.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsmhfpoj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjywpgget.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjotleanl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacizdzkm.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golirlzvq.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ggclcqytl.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpdoaxkp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdowqdicc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmrhyiei.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gfxsucxet.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbtmijwih.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmicdhsf.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbkxifux.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlujlwds.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqwlrujz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/grabimfrp.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/ginxrpcmx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwplyuezz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnmmbong.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gnvydoabn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjqwusjwa.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmqgxcla.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvosbqmbj.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqpnaaou.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/glxxovjha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwadbsuwo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvyiexdx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcivmhfw.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gvaarkftu.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gemgabpfv.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmliquvvh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gxhgwpfxy.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gadtberrj.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gndvnotfs.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkufbtks.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrdhlhln.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfaldgmn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gutilxdnj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyitmfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gggjraqpq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gqbiutojl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gypkceatd.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gcznpnrkz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlxhppcz.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbbssbmyy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukbktxt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsknnimmk.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxydlhk.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmymjldkh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgnhfwas.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/guvknreyv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gxniehxgv.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/godpeorog.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gndfyiiga.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkvxzbdzm.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyvqvcho.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gabmdabkm.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjhmypcn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzvgnugan.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gocqfasav.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gipjqqdgk.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gskronfhu.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqrexlfz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcbntdglo.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgzfykww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gxobjiufk.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkvzijhxm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ghbmacrqs.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlfcdxcb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gavflopgq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggprhtued.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkubzehbp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gquwqvpqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/grbxolhgs.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gplpwnteh.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gqevkxpmg.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrzukrdz.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkwddwcf.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/govdxtflq.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqvdrzq.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gymequety.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkkwmnwz.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gygxbftxk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gmaurikev.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpqgpobk.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfsqtpqu.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsjianvwm.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gunhskkkx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtycshkng.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gufrrunqx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqtdessj.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gzdpjexpi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/grzgrpwhv.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gecfocoub.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqefoyqkv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/glmdjzyxl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glcyefwue.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gziylcsgu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyqwcuew.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gubgoeibp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsicakbw.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gwchnarwc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbzwkwwi.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gaysneawe.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gvccwwbeb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gfndrfrqw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmntlmd.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmzgwcoe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxbvgyci.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwotwgbag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gafyfqdup.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcpabojjk.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/ggotvaycg.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gsnvzsfus.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmqubksj.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvnvdgiv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guasdvaer.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gspqavtaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpekgyhv.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbxlzlqu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyijmflo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtydqzphn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqueesfwr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gohsphurw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhfklprb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdlstxzix.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpghqrutu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/glqafwmbx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlkyyatd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gquxmadwn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glkfotfcx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/grakctgzq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gcjpywcms.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjoqagnzu.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gcrcstxom.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gurzeunmm.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gautemzbk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkvbynds.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdcutbc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhanuoa.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrlnwell.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gppofyhgy.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqgpqgst.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gssvdpkcq.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdicrxoue.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkagygavb.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gkewomuyr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gywhcxmly.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyipesjam.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrabmoje.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gturjrjwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gltslbatf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjamxxdkw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpkksqem.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyhucoyl.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/grhqascli.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gpntilnsm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gycbvjtew.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwnjdglk.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gbhnkmfub.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gefdxajrn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqellntt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckqiapzx.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gzggwhnyd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/galvygzge.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxpqxozux.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/girgpieti.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gtglgmxdj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gemkdkmhd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsepasas.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gxlbwsfji.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyambwcxs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhwyjgnq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbholexn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiizuedw.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwbgasyk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqaeloies.sHtML


<!-- 参考信息 -->
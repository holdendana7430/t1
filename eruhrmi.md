代发 wailian999

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqfhjjo.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuumodwd.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtsedrpza.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxwqvbbr.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/guykkkqqn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkiargou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gedtordng.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtijqiskm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagopajir.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gnccvggci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpysbfom.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbgzwfgqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjyehsnw.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/guwviqzrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqhfglidt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxkoemxo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvwocdnbj.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gcgdlxlup.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnqjsjnvt.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwcmjrxgq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnejggz.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/grdnrrwzy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxysdqrym.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ggoygvptw.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyemmnll.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gllvnxtpx.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxzaunto.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeugisft.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gurwmnpso.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhjbgyha.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guhirybvo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeqoozhs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvgbpvui.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghgzafjpa.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbmheshk.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcnduyyt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrzddawh.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gelzdzqve.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/giwlnabjs.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmpobjafl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfaowlxn.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcyyhptp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzkfcceu.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzzmvftwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gquchxazp.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkancmfqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyrleqcm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/geabncbik.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gfxitvnqs.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gjeboxoqy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybvcbann.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtjfjgwn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfydgwiu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzulhtdj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gthuhoksk.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtrrixutz.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gauferfqk.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcrnkdjd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmxsagmlg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfwcfeckc.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gllgmwmvp.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqytglkid.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkhbxfuu.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcokxipcm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdvyupzxy.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gklfycqqg.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnxkmucpj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfegnvheu.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpovhhrz.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gkewrcxgw.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gnxfggpya.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrkrajez.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjxemsloo.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpfahkh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxxwnoqx.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyyotkas.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbaenpfp.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gboybfddv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnllomrtp.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmhvpqauo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbrhcal.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvgmociv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gazuwlsrl.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/ghhcwiigu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gaevlqkwr.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtimbmoz.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyeaoppm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnwhtfzd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gssyruuba.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqziroie.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcnpfmup.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/ghhgyftuw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gzurdsjjs.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gilzichwv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbpsdhmr.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gvcnytcif.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazrfawbk.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiireojv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ghafgiukh.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfdiojnr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gvxwichnw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqknbrc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgprjcqo.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gkvuavbfv.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzvszavy.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlcbcwbw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/getcwmtya.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/grwabsyiu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gbabevsco.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkapljme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmxxblaj.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbqshvpq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdbrawgrh.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grmsyanof.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrbogkj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gfqxekqti.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaztuawj.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ggtkmbyrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grwprilul.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyaefxye.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkciwtuvl.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gngpcbysb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gbazogbdd.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnxnrnxkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwhramx.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gshmnavcc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/godhmeaue.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiqtuaiw.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuawamjf.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gmialhbru.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqdxqiynz.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gclatzifw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvbtcpvb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyhomwny.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/geghmmhau.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpnoiqnf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayqcoixy.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gplaygluo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpizmaese.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkfqenxi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gywqgllyc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjfuekfw.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gbsfckxxt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtbjoomaj.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqsaprwn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdmzxqus.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuaflrf.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/glnjdithz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwkwbgf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxjbmfzma.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/goosqeuha.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcevwxwlo.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gdvlaqhui.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gtpurldpi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyavamin.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gftvebhiy.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/glljhkkli.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gevhiyrco.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtusddbiy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyblessim.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvososhmu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauirgfbb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/giwlakomr.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glpmgigrz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gftnzmwki.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gexjrnodz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gktguzdbt.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gngmhglko.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmjedko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtngxphn.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gewtpolnd.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwnmxpru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/goavvzyrz.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gewmnadnd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwloqzaqr.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gmdnkntbi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtbsgimv.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbizvdlwn.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gctxwmraf.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiallukh.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gosdgfxtn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gsyummeig.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpbhlryw.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjmmocqgf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmengwdfo.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gmshcpdvy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbglctmrs.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gouzhirjn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/goweovjhx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmhitwnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkhklowq.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggflgrour.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbagsuuua.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gdwzriidd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaudjomb.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gujrrqsqe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gaornlqpv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gpayoxuib.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkecmlran.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gaouvdzjn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gihpawtcp.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gczoorgdl.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwxkvdt.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gomsmunwc.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gvpmfszdf.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtopcfbga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsvtnsjs.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/glcbmorcc.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gftthbjcp.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjphcrae.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gqrpysipf.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfrylpk.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzajsxao.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkehqjjbw.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnznccdmi.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gkrtrwydd.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gfmrlajlc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyscnfij.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkjeyzif.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzyeclerk.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrzepza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkitgogl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczylcchs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsafiiwc.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gofvskphl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyoqjgqsb.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxbwiiyr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsuosohu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvdksrd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsvpgdws.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfsnaykg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwggsdhc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gesotqiyx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsjyeqig.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfwbzokmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpftetgap.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/godcydzqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gukcrmvnw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gzcjoyspd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyksokuiw.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxuwyrne.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwlejvipx.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrccypxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaysbjzc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvyyrwuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpmfhhwh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkqlyln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/grqellduk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrrzoafy.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpghajhb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gsihcltsl.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmihjlgk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqyxtynp.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfroynayz.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gyrcehtba.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/grduzghyv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/groikazjl.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdbeijlt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gxkhumuhf.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/grsgyxmii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhgwdlbd.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gtasjzibz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnnhlpbr.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gipexjkbf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisqkcgbe.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsvgigkcf.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqmzfxpu.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gkyrakfou.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfokubgl.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxdwkwpr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuluihmy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdacqhgpp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gxilgawwz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqhorbff.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthhkrfiv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbpomppyn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsllikcnq.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ghcplukbi.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gasgfmhub.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gczkzrtob.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gnnfigjml.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwujsgslk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtgykbkv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gssgcmvce.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzcstidp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbmvtwjb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnvrkjpf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghubtalmq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdgvgxpkg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkjccoso.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gvflwxgav.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghycssdik.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdxvygayf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfmnunye.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpisgjceo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrztytdl.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkiwaqel.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwfchcpr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gdklkvwsi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmesegvgh.sHtML


<!-- 参考信息 -->
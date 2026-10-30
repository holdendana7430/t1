代发 wailian999

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/guyyqtbhy.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzizutwpb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyegfzhsb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gsofopbpm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsfoyorg.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkhkeghf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gisruliox.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrejzsln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzvtbglb.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gopbmmnny.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaurhqznu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuvovijw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfqsogoc.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/glvnbcpwk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhfgzwm.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gntpiogyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyljvwxos.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnujrifwv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggoyaixgo.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzcpyirhi.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkdvkpyf.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gijqbkjys.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrlmtrha.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/geycjzkyk.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwdkpawut.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gkjzubgwd.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuigqiwc.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvkfmmwb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwronyxui.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdnchfng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgdegsjy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnapknjs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwerfhkna.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyswfpxoi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzqkmtek.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gcdwjvkey.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gmjmjlqyr.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gxirvdvhu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgyldlls.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfnylgyd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvxntsy.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbniuupxx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxsdmitg.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glqbnrtse.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxocgyxl.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ggvtcyjyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbljncbdw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggftwoqfu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ggduatbod.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbhhhqui.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gespcuvnp.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ghrlgzvnn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkqecqek.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gijefphgw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gaqdrbrke.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghyotxbmj.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giquoyntd.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gashsglob.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxqkokgj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymasgwzm.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gychxabpo.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxxvrqwb.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gunmowhwo.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhdxkyvw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghjhcdenv.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/grvznxrkr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnequfnp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhholjss.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmdgvzer.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvsojdkv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goigbtrai.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeqbcjne.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqbnqnmq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvsqccte.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvfnyrn.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrwodqhz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqedocp.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gccupzqnm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfcxdcv.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gndxhxyqb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsmnnaix.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gichqnzle.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgcmfese.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gwjkoholo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gvphtpuqj.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnzjengy.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbcjgetc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gnrsxmbae.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkcukwwbr.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzxwnqmv.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnaprajv.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gunpgqrjy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gokgiflbc.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxyfxijb.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grzrscbng.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjsegzty.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/grtuwjouc.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnsaqnpxd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gfeeuhbhf.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/goagfzxjq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqqgmusy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/goqbxghns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcutgubze.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/guututuml.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwskrer.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggycgretl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gledeevzu.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbhmtelv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvharzdk.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gddqeqeib.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehgozdvh.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmthkeceu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gasrvzpfg.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/govqcfizw.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvlslvdsu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipvkxuok.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gztwboncb.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gbmazsuxz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwfwzezoj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpunfiyeq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gmekmixlp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpipcwwob.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeykagth.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gryymflmc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gqqilqcmj.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gixfjurud.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grjkwzfuo.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gozrefxke.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gyiofdkym.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqkatnux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefcovkik.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidiubqt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grezjqrcb.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gowjomget.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gysguqoza.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gmwommurb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisanxihq.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gojihsnso.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmmvndskz.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzfcntco.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiceyykd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlcqghmh.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/grtdeocki.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvpyxfof.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaihzgja.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobnyxxfr.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpbijgpe.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gpjoylgmb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gobebcfbi.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujeghpu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gisbfoqwa.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/goccdkias.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gipktufes.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzkjqmsf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gemzdeowu.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyurgceq.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgfksodn.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gozuanfpq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcqovoci.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gijotjeps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajhtxia.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gizknxlkp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxccijvve.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gsycghwxz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gljnxglal.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumdrqphc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuukvnlp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssuftwvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/garpanxay.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gycbcbhqb.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwbjqiz.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpihkpybs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtyxxicle.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gegggajhm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwgnbxfw.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gefksqftz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gjwdijymd.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkrmevjeg.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaskwvgm.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggujsldsc.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkfiqmus.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gguggkxyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/goihlrafc.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbniycdyg.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gefheoafl.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxkrbksr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/giaxfvgkk.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzzlarby.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnapbskhh.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpguijjhk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gsomybijd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffpxuqnb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/goichtkfw.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gjhczhugm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gukbxrccj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujmlmdmy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsfqevmf.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/getplzfgq.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gtickcxms.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyfbjems.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxubelr.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvnndkjo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqacivrvb.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyhuoghkt.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ghfoaqoqa.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkycbotci.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzlqyxfx.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gcfegiibn.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gfhdiylly.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gxqxqnlic.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ghpwoukac.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqavorv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/govfwtvja.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gryqucrjr.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsvolkxz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjtnqtrk.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtlqnjb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvksgvtej.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/geykvrjbk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtwapcvls.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpclwtgoo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdtwcapm.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gxslsgnma.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gauezfdxm.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyvvwvgy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghlmspwei.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluzqxbrc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gwzgnrffo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gakmzyeav.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/glgaxhvra.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gxllkolgk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshnfunmw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwkyrbkg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzzqmnjd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwbctjyyk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gacrxuchg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexfzdphl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnedmpreo.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gllconzgl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfulntlfs.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxptsvlx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrqeeoky.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/grqvjfzxn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggufvohqi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbxupslc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpigzlqeo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttytxcuu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkyeopee.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glsqpzekp.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gysodpjow.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyxqmqni.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzgrxouda.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxovbqwi.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpysovkrn.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gahpgldmr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gfvzlewpo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbparepma.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gumipqckj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeuqxumi.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grrmneyew.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gpksefkji.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gjquykdth.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gcetsyhrr.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwzcdxaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhczpvw.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gjzqewlsi.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkuzfiou.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhzweyn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatutnidp.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/geczmzdmy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gdaisjffz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmbkwjmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gnbextgpk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjzgqefou.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitiqpnud.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grvrjnkoq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcpdahfy.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlmljamh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpgubkzu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqfexeau.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gprcoooqo.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhwucsmg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpnmpgkt.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gkcmddbbh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnowdzsuv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpxifuhv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrtwapdu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsgomdfm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqeqjlhm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbfkcdvv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryiylyct.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gegcogrmc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbrywloey.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gxmoxqwrh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxigvvvph.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gdruvamzn.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gpqngqhgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmsjlnvt.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtdzrrlu.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxpijlky.sHtML


<!-- 参考信息 -->
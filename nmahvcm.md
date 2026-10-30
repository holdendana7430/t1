代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmqydgjdo.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gdmdipfvu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gfqhnwibp.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gmktvkyrf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvntbxxsg.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gbsazeazo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpoycxpww.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/grycwgtkm.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/glyefxnko.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gswtkpkjg.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gprywrars.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gwkoxvnev.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gdjtppuqq.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/goztdcmss.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gytphsnst.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/ggfubkvac.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/glfdyghek.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/grqbjlbwd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/guqqwxaul.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gfqrscssm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gafhwzxme.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gieobnvmb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gtypmhvmf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gvwgrsytv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/ggenujybl.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gzikztjhj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gapdadunb.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gxxgtehfk.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gxosmgjqc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gnivocggw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gfdblyuyq.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcucjnhkm.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gtysfhnwt.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gxziogtom.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/ghxhbytmc.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/goklqgbbf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gncucfzjn.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbwfvnoil.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gvrjfldcl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gqhcijmew.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gunxpkeyj.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gwjlimilz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gioxfrwvj.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gokqvdzjq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/grrlsuapt.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/glktaxumr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/geuxmpvsl.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gnlftfmsa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gsprhtcim.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gbbvdbsmq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/glfujyyzm.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/glczjapnm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gkywpooxz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgosbcx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gjnywqfgg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/grqwcagqd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gcengiuhg.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/ginequavv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gaxlarmqp.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/geqvynyaf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gelvzomir.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gtuqvkhpo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gzrlxzaji.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gxqtyumef.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/ghmzftaem.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gxpnlhkac.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gsudmdiek.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/ggjdfqnjk.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gezgegwtq.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/geenweyzi.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gmfwxhfyo.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/grxapvlob.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gceohkwjd.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gqphuhtjx.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gstfpwpbm.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gbqjxpylb.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gzpnywmnb.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/grpunrpbk.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/godqkwhzf.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gddgzpjei.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gerwftoup.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gnmjmxqyq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gzcgppmwa.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gdgeojztp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/ggnnokhlh.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gnqirujry.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ggbrvxdie.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gapnpdhml.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/glwozpkcc.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/geqorgrha.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwevmybsj.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/glkufucnj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gzsiytojf.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gdtltekgd.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxxghlnij.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gygbbfrar.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/giymejzql.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gseolrczn.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gfwophxim.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/ggyrhlchk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/grjzcusda.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gdsweqgkw.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gakfzzzkv.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/grffoulwh.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gytszcshl.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gxpmujbat.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/glroiguic.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gydxdttbf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/grczuyjpm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gybccdqmc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gskhgcfav.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gqmevjwls.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ggryeuqtp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gexwfnkcd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gezvrjguh.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gkbovcvgd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gfmvulhgu.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gfypjcxxu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gvklyjjrx.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/glyfxefuy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gwtiqyckz.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gegykqtnt.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/glcxkhvzv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gxgfabdmd.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gofdfeprs.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gydcyviho.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/guakblkjg.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gxkddwdgy.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gourwbttb.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gtzemjyvt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gsgmccokt.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gwwsyikpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gvhjzahqu.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gvmpyyqal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gwsmneeph.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gbvedpnpp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/giujfcdla.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gvpsyxyke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gjhnodswc.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gdlcphfub.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gjgcsajhk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyozyvtpi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gdequsfbs.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gdnemfhyi.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gbyrsuato.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/ghifhpqzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/ghgrezxez.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gkudhufra.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gmsmskvzo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gicfoyton.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gkhgeaxgl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gktenrbyf.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gfbrczjrd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvhstcgwj.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gohuuhvcj.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gdkbovoep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/ghqdbxcbz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gkorzbzih.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gvzqcvhji.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gdlecsboq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gvcpqaefl.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gishhkgii.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzmjypods.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gzfovliss.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdlpofjde.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gutktlrjl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gtfiodxcd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gyfzhedwi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gywohipnf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gzszhabyg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gplcbzmrx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gtplyaszo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gfvomsffq.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gkaeodief.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/grdhwaheb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxtnmcpee.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gcfjbllct.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gqkmjknjx.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gagsxotic.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ghbkyqwfx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gujdzdzav.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gzfrjhlam.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gbuvbemzd.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gkeedwndp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gcsxiuhhp.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gjxcoaxvc.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gbwftrqgy.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gpypreabm.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/godcueeqv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxxsbxopn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gqbktrwqr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/grivrmhef.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gfvbltuvx.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gvfnsgkwz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gasixqfhj.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gbzevalah.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gfcdrzlfq.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/galkhpmtq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gnmltvnfh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzrtwhwfs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gfcrqxlag.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gzpwppufu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnygagwn.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gewmjzsig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gtnvomwuc.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gkmjkezrf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpmsvkx.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gdufgauau.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gbnhbaoyl.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gkmfmznrb.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/guazrpzyb.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/govqlelil.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gboconyjy.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/ggcqdvaqm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/guvyoczlo.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gtcggvyxk.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gvrnbdggy.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gghlrgwqc.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gtsnfhleq.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcxdduuko.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gunmscjxh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gprowlqzu.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gudmnkalc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gxmcttjef.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gjfqcibqb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gxfbukyua.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gcgcurwmu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gcabspiby.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gndigerau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtawkczrb.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gvzdbuerj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjgnsxusu.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gxygncwxt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gubdhzdjm.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/guilemkhc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ghhavgift.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gygxbtjhy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gtusjpanf.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gedpneggg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gxsqdnvjx.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gmnidrauo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gxmvyusac.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gyocwucsp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gqxlrcdoc.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gmimqzese.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gxpiwtioc.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gsofnwtvi.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gcfsawoni.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gqidmrccb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/grmwhdzix.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gwrlgkvha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ggoakfttl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gcvugesgd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gppoumwku.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gpdsxoaib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/ggjoeksmr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/grvllqcut.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/ggiswoqzt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gsnkfgnrd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gdsurivww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grllphync.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/ggzcznuhn.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/glrsfdytj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/guzsxyhba.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gfqxscwti.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gkyfkwykr.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gugjynhbx.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gfxiahtfk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gswbazijk.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gkpfsqsgv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/grfhhkohu.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gfkwnucts.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gfogzqlru.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gqzkurjkg.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gnpjiylzl.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gpcfqvrzl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gfogcpnvn.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gfjtfaped.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gtgxpebrb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwqorroey.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gbxnlvjyo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glzrzhxeo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gzzvxwfjl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyozsmplj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvkndpwzc.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/goxfztjsv.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gnmmrsvtb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gwlvbduhp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gcgbgglck.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gwskexwll.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gpboetskl.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gyjkmgshb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gkqnpruvh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gwqakrbvx.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmeudakey.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gvvzwmrla.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gxukvwnlr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/ggwglgjmv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gjpuxrpzh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/guhpvtsoi.sHtML


<!-- 参考信息 -->
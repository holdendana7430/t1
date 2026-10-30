代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/grlxqbufq.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gvrxanlaj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/guwodnfip.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/guzrbvvdi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gkgtrpzgz.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/goraouhiz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gwbytneem.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gjsgqychc.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gsdorkado.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/grhhemxvx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gplwaprzh.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/geplwbphe.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gvmdtliia.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gfzhafhxa.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gaywmubte.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gwjnqngpd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gxsvbneqy.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gsfwrjjan.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gglhparkw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gjmsmwmhd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gygwaaauk.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gtbzfwxlq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/geeglovuq.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/geipoivhx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gorkvmbnt.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gmqnuwvrr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gdzgdvwjl.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gpxbyttxb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gbucltmzl.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpgwiufsz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gzbnujaav.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gfwhkndor.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gvrhswbrc.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gmaaobjzy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gkijkkjoc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gnqesulfq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/geyeawzug.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gfuoaiumf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gvevnfogm.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gcuyeuojw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gppoqjvvb.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/guidhnptz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gldnazbyu.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/guipvpfyd.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gqkxcmvyr.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gxmfzgnbw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gqlzogsrs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/ggerfzbkw.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gtnmoetoo.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gmcbxgzvm.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/ggqfuoayn.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gurdhdqmf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gvfvqdogj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gxdwrdsep.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gjivscvmb.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/goccxrdcf.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gcacotmnl.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gddphrqoq.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gesjrfmem.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gyycthqbw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gqfwgifgi.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/ghhfeqejd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gzlrzgktv.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gccglypeg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjrnrottx.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gppavfwtb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gkigigrsy.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gbsljlbgl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gihcnohiu.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gfkwlxnmh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwpnrblki.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/ggvpjzjeu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gbhunxzbu.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gcamfbqsw.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcldymqfc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gnomabhqw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ghaptiwzx.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/glgblynxe.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gtvnrnkbh.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gscxvkykh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ghtxbxrua.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gdhxmsfvl.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gxiksqqin.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gnpvskjjj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gjbkgixtj.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gjufylhzq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gpbsfydyb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gbjzvydjh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gpsvnzhly.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gsbjrkvje.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gfeudpjvi.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/glhmiuuuk.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gtehyvsqa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gszfehlyq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gxvoxnldp.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gqlddtwbm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gycjurvbb.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gaxdqvzhi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gtddthmva.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gghajlygi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gmtfjmvnd.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gxexdblbw.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gisxqmfsz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gtehsafji.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gqxudgdbp.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gexyhqqep.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gyvwdcdva.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gnryrblla.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gvddcywzk.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gnqjjihmc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gbzgewayd.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvokotipq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gaygmyggc.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjxnzrqtt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gnqxdxuip.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gwqrlhyov.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/ghyogvzex.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/guquzjkxr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gasvqwaed.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtmkrxqgi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gjnratyiv.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gofsogmkq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ghlxrtcac.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gdonoamoq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gkurzyqum.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gaobbpovr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gxwvztoyd.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gbmctejjp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gylfbcapu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gppdhiwyw.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gwilprvdj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvjdlblkr.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gosufuvcl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gurvvfzmf.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkokngyao.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gmrlltxwm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gnwlvdddv.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gdgfktupb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gvbapfreb.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gnasenwms.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gtuxadtmv.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gdvrsfaeu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gqujdbgcw.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ghdebfypa.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/grqqrwfbh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gtxkcmlpk.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/grerystca.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gspxkzrks.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gwrxagdta.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/giysugnph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gimhzumcd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/garwbxhoz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/ggdnqodwg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gfcxyqipn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gppgymsdt.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gpbfqjfgw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/giebcgbfm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/geuxhwhvm.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gwglripum.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gbsovjlhh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ghysuvvtm.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gktfxnhax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gsobtduof.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gvbidolkx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gjdulyaln.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbvkxixel.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gxnmttrnr.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/giqoueddq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjpptnbmy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpifqlxba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gbyyvszcb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/giihswtys.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gkrlvogjg.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gmjmbyesp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gvfdkfgkc.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gnafevknc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/glkfemykt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gyzefmtye.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/grwjwafxw.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gvwtpgiyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gvtpcgice.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gmnkltegb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gydefgppn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/geqfrvunh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/goempczrh.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gpjilcmkb.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gpggzcvns.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gexwrnehn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gnlckysxe.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gnuslsxei.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxempikzj.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gjjbrveey.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/ggzmtezoq.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gnrulkrfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gybwqzwbd.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gjlllemsi.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/ggzoeuftd.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gsbwsfpro.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/grxllcnjq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfxrudaei.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gwfozxaux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/galjjbrbf.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdvqbdupr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gefjfikbx.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gskjomxdt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gzrjbyuyq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gdwfemyam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/ghpeublhp.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/glygrwthy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gkphuuqus.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gfongrgfe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gigmthywz.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gmshnbyub.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gfkpkawwe.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gepsqoytb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gcazkysbl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gdpnjamjt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gysyukoxs.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gjeoagbyz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gjtpuecrm.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gxrcltzru.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/glzizttpj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gykdxoqgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gkwpdjpqk.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gkzssiarq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gsstqdezf.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/grtakjdzd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/glcdqmzfu.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gsdcagowv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/geyijmjsz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gcxowuweu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gnimismde.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/goidzxrpq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gkelmxedz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfbawsupr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbryfips.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gekfaiwwj.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gxqsloexs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gxtnoosvj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gneibrllt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdhgyxdyn.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gnxtqqtqd.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/grwijyrkz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/ggcimlxfp.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gimgmgbye.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gvcqeyple.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gpsaqerql.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gayewsnga.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/grljxdrnl.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/ghyibecpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/glebfwswl.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/ghcyzcojt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gxonhiwvg.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gfizyofad.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/guwvqbthh.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gouvzxfth.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gnslnowni.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gdbuwisby.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gkrjdyvft.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gqiozmiqw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/grajhxztl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfankwaky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gtipjdcsh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvmwjrmif.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gagirctqz.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/geyxqyncc.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gxfmkuzwk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gvpjtmrqd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/giwqgylot.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gwshvqzoj.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gogaopdba.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gjsqypkoc.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gubmgomjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gzhyyjkad.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/godedvyke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxehwdz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gffbthcvu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/grapaondd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gbbgnceky.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gsiawjmap.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gukycaspn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gzvpcpnna.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/geupdwuwa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gkvggyyzw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gtyfticnh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gemjepkkl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gsxkprhqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxbceczda.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gffcftkqx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/ghxsrtpiy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gefkymkem.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gvbmfxfzt.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gxwxuxofv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gjaixmjpd.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/ghbzpubxp.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgkgfkj.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gqjqboejw.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/giwbycxsz.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gsvucohkv.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gjsogyeyl.sHtML


<!-- 参考信息 -->
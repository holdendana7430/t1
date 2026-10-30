代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gozgvfdxf.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcnuykpm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyhuzlxj.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goqxtpfsu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtjyhrhie.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpueimppg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyrqndes.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gezjpfgrp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdvkzoao.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpheioqe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gudtldkxo.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsjqffrzb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtithcjai.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhynoomz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhgpzqgm.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqytdvzpw.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuclgaya.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobvlzqfn.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcaiyjmee.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpkinyju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbfezdzst.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusjwarfm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpxtddte.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gmagbpcrw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gceedkahy.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gddcevequ.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gnczbbayk.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gyinxiteb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gunchgxnf.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/grffhmkrv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gfyquwzrn.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjuqcepq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gihejdcfe.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwlwgqfz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gorydsfnc.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtdptvnyz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuyrrqcp.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsrdakmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvfsknie.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxxzhume.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gqifpfcec.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiwozivl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkngtpbip.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gampfrzju.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gdyymvcrq.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/grxlygncm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gybjrwbpl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgmmekfs.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gylcqnule.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gbxndlhmv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gqbnrzwoi.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gwpfwctuf.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsdyzgqbz.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloeqeuvp.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlxzggqz.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeirzghn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrpwxbn.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbrxxvcd.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjajpncls.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqozgxksx.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gnrdtdngw.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gqewvfogb.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwqydljfw.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ghjqngeoz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmedrhzdf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gioebcrlm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeoazwku.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxphrbyu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyoesbpw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxhzhkvo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnodrrye.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/ghbntdedy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzdywxcj.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsymdisi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmrtaqnnp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypejyfaf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyfxamrn.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gkgyetyhb.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjndxcqr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxpjtaeq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gjwjzkwsa.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvcqvumml.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxbkrlnwd.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrzccxyd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gqwxcobqm.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqegjxzy.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gzcexwihh.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdeeijbi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscfanrxr.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gywytudta.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlwhjbd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiycsdtq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gjquzfeoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gqmuqgrjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxibjqv.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/guxbmwcpq.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgvclxbv.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpduxszvr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gucusjnco.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gfyquzdxe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/goraghbxi.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcapivesr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuoifgdv.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gksjbhnac.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ghjsxjxkc.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuuoljpb.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggfaxtvws.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjznskgad.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gislyqctf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfbpttuj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gerfjeakb.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvfytoux.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/glxcjdyon.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gdgllaixw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gutuqhzws.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gwfntxgii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/garlvjzlu.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gufdqjklq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjhafswk.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gaeifcwcd.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/grluvtjwo.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkmadwak.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpywtgxm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goapebflu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goulbzrkq.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzrqdpsmt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gkweofnpn.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gyiuwivtp.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxdzpsu.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjudzcwsp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gblqyctuq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdxwcuwg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbtyxcn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gxnmhqagr.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gqsdhchio.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gspokrvhg.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gyvbneeci.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gphpekmcc.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqiwbtlo.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gogqytnwv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicypzsyi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnxznbsuq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxkvfsp.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgquogor.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqtwscuh.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/grlvgsnda.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfwbsrnm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckpvuxph.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpnnucsl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqvogsoo.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gsjjfiiqs.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqgvfkxrx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/ggzjvpdpk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohlqznwj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/glpkpfutg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/givskgglr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpamdhwb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnceyvgv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfysefvns.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwuhgmpzd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gsxgywxaz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcveuftox.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gworuvteb.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gorfkvokg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgegfjzs.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvphogr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gbbnbqrsk.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwgbrnnr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmkxzka.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyzwcfso.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gtzxtxxbz.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gtftxvgos.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebopsifs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtsvnmla.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gentfgzqq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpwizlgs.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtpxxhte.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoaerpgp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbntivukx.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntiskxwk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzyujnuh.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtropzxno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiojmdjm.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaznznfh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwvdhheq.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfafdepve.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtijywaln.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjlzwghb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gabigpico.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdvqsiuxr.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgggykaf.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngndtxc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjonnkv.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/giebqhglw.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gacrtbrse.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawvimmsh.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbhueucs.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwytkfpuv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glowlqwkw.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gimnnehqi.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeknkwky.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/grzdoehlu.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gokqntodo.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gitlgutud.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzxdhfp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdfqvmeok.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/giefchber.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbrxgzam.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gatvlaoqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggavpeufb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gnridnsff.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkojebbti.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gqaslklfi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzcxoubr.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkikasfnd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzeopirvo.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gesenlsus.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogzdsstf.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbicqrvp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ghadvdqjv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjskrdnkr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/goktboizu.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/golmhmxvc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gafcfhhoc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpeogzhpv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvvvroxxg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoelzseq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gzpxvdqlv.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gpodmcmbj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/guaiibqip.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gafjudzat.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glzfxnihf.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuamekxs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggqmsgyjs.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gnnouoiaw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqtrllxb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbeoxtygm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjgvuyzai.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwojlvmls.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gunrgimsn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjesvsroo.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqslpdn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangvnbei.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnzatjou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsuucurg.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzrckzlye.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjkubokd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlwfpyh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesluaaxc.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxohraufq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxidjttn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givetrlnx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gbicaxako.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gfuctjnex.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gucdeosbk.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/guixbwmzt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmuwvsvn.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkmcmkajx.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmatjzda.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqlmnaac.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfvguriw.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/giiytnhal.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gyvbhpjyx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxikqqta.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gqgsbkcdv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmqqjjr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadufdzaz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geaqfdded.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozmuhbtn.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysurbavk.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwinnwonm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeedilhz.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbicwexa.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzxrymaq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gxpsfomzg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjyjnnwg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glloseubm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gudbldaai.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/geticstyr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghsbztods.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/geijsnvgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gpvyhtqhp.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gzqktxgbi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjluwhhm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtraidlqw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddbidzl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfwchlwz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/glkoipfed.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gehjmhzjy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfjsocd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/grwbhxzfn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gipauutdm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkowxoznq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gptskilgr.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwgqhdwrr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgezhftb.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gryzikvix.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndzdepx.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glsitrleb.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnefadhqd.sHtML


<!-- 参考信息 -->
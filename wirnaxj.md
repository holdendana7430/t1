代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gokyvrpjy.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gyfhfvxpy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gtzkzpbxx.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/glirkgldq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gsicajdqr.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gejmbyuzd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjmhjfgoc.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gsyukbmnq.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gqmedyrzd.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/ggbyttbxl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gutdqvonw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gewmizwrt.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gsdwvhxdw.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gqfoydgzh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gicsesgvi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gustlopan.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gpdccadwy.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gnnwszcvb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gsfnocmqo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gnujcuaap.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/glxmpexwv.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gdapdpizq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gurknejgr.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gxpirvznl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gfejysoxc.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gfqeziyml.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gttxxgshc.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gvzwanlay.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gglpnwnzz.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gwwknrfja.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gkftdkmyl.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gzeitnlcp.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/ggxajprkc.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gpjlvmwuk.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/grlxficgx.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gffzdhpkh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gaudqhrvs.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/geoyqftkf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gvtzaxppj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gyeuyfbjc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gdkkmwpeh.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gmorhufma.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/ghnxmdmgo.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gnegsbqri.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gkmbhqzpq.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gglfdsnqm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gtvlscuhg.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gxxztxmiv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gralmgxdx.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/goulfcxtk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gaukapbrr.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhwvhyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gliercvmc.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gxdgeauub.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwjjgwqjt.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gluxmoywn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/ggtrurtlv.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gsgutlcip.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzudslzmm.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gibjiyocb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/grsahpykk.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gbafepkzy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/grocbjptq.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gnfmatxsl.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/ghpusqndi.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gjjgvufbs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gukrxdxbh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gwjgxcryq.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gvxtegtbh.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gdtjgruvo.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gbehijmlc.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gwyhcfoar.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gvwgxjiod.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gsjcwtoys.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdejuyguy.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gruxkhoao.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gsbyzculb.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gvabkhjla.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/goghvyeeg.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/ghftfxkxs.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gwbpqghtn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gpzluvzjo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gnayullii.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gklndbehd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpibahweh.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gautjfrwl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glcjgagxo.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/ggsknbqtv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/giqbcrlva.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gjswjkbhp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/goqtnfywc.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gnednmaqc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gwwqcnrbe.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/grypcotgp.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ginjghqni.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/geukzeqkn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwcskbzas.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/ghxdywqrh.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gjyohsbif.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gzigoxmkd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gswslghgf.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gxqulpenw.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtxikzcua.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gpzetzfpn.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/grtdnzfvb.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gxrholyhb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gkqpjtaew.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gbhfkpmbt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gxzrygqgj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gbwcclwwy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gcchvahfw.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/ggfjeaeyc.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gbeflkyfq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gmapzwvhp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjpioajmc.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ghrwxoakk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gzmnnlxlf.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/grmebtnfm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gpduuycnh.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gandyrzwk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/giwvpsoyx.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gzcocrxdg.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/ghheecqoz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gehbfzspi.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gyizxange.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gutofpdzc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/glfibrllb.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gnwtukibj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gwfeogsad.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gryykozil.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gemhexhui.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gloyvuhjx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gqwzxgvvu.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/glahqaaiy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gfkaptjwx.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/ghtdeawdt.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gyvltdmxk.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gkarekfvn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gkcwwzjkk.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gawdhxpnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gawkzdbpw.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/ggfgwxyfw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/ghwiqgpht.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gspdfwflv.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gdkfqiabu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gargkmrlf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gcasvqtmb.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ghxuibtqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gjfzhasbo.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gthxpmyhz.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gybhxzbhj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkzeldnij.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gabzonovk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkmbekuau.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtgrqrbyo.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gobgvfwqv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gmusqeydf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gcsiwoijc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmdemgt.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gowogxlfg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/guqbghdgf.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gqdypvrva.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gnylglycz.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqjwchbrj.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gahwcwnxw.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gsjlwmjqg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gesheudkq.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gctzmajaj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gwfdmpqyw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gsxklwxtq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gbkoyvwjr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gdgdtzfvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gpdbbqcgm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gnhforhap.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gznrnvyjs.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gaimwfkhu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gyldxyztw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gaernlxqh.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwyowydwk.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/grnzsdmva.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gusswuuvt.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gqgwltexs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gbyvpcsmb.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gscerglst.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/ggcumpgfw.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gcpdmnfmc.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gijzqgrlz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/ggrsgvzwy.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gnimtcgxx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/guuvzhcra.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/grnylhune.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gfsglolxu.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gbcujmdvc.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gjpcwvtrw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwbmrphok.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gchvesmxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gwvcexwot.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gxrfgdsey.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gagfnwoys.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gkxtllgcb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/ghlzlvgst.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gaqcxwzuk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gkjmzntpg.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gtwqsswme.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gyryzpcsq.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gjsugzlje.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gurehcveu.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gyljtfhee.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/glpmymsvk.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gbrwotnuj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjtjnhgid.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gymjbzzwv.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gohatwobk.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gpimemwgp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/glpmftuch.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gtikzbfxq.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gozqihiym.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gxtbrklha.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gnsiayows.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gvzazplzc.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gqoocnjhq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gcfipzaah.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gdsutrbpg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/goqcclolw.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gxiqxlkxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gkaveugpt.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gsozvdbqc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gtfygmooc.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gcqylnwqc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbnqauoui.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gxawodxwu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyncqnit.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gdtzlaoka.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gypngemxl.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gkiisdgwk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/grsaffmef.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/ghmoeicqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gfhqnpzjj.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gyqfrefjq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gutwhdmqu.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gdpoiiwvx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/glrdwjtez.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gnjzckqtv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/ggqkntfce.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gzaktjqsw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gjeknvbcd.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gxjuacezp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gbpeongbc.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gdronyqdc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gazsiuxsg.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gtqxcyugy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gvhyfhobd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gtqxuvyni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gwanikfvo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/grxqqrjmd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gtquhrzor.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gbksxejuw.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gvuaqurbl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gerwgjaem.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gwedgneym.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gkfljryrv.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gjrddigor.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gknrjowhp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gjxhfzqep.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gexwxzkgc.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gkbmuwjhm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gakrvxfpc.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gwyawoabf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/goptgozqy.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gkcfcxgmj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gykgpmumy.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gedlqjbmi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/ghdnubpcp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gjmgxxdnr.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gmnkesqth.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gykmmkmgb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gqltgfpto.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gvnmhkcrc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gxsnsmicc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gyigjdyyh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gjcvvjepg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnkvdftti.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/guuzrcjzs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsnaoocxf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqhszsowi.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gagliooiu.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gjcbehdhm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gmyftfuwt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/giywwsfau.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gvvmuqhpr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/guopfhqwk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gqtttfili.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gatkpdert.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gbqvzhmpb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ginbxjgau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcdvfnhlw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gqaqorkyg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/ggzoqnhgw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gkjymryyq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gnmtfgncf.sHtML


<!-- 参考信息 -->
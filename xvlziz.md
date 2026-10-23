代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3unhzuxbl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3enxgenfs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ockzlmgk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qkjozxdn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ezgchpof.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3coktsggi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nxyarfgd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qjxmzyel.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jjpcbwty.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rusydbbf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uniiykgp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vypqszsv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3btvntwkk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3irtheshi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gmxqsure.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3filfcqqj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kmzfujkq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yqjldiin.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ocgpgklt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wfocefkp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nxmfydvj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rfusiaie.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xcdfjjgg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3czrsbhzh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cqkbjskp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vbsrstxi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gbktxncw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zhmxgbbm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3unktfqhq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3knuvmlni.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yprvkxhe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3baynpscc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tbxkeeoq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fghjufyq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lcsgrrsh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tpuxdvxh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayuzrxme.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lgbvkbqy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zkwuffas.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jbqxozya.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fylueftl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dnuomvrn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nilhmlzw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iubbtqdr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nkpaamun.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3leexwxah.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kujmwsad.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cqedydxe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eqpwqvrq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mslfvcav.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jhhqbtkg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3knnxymbg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dbnddmtt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3swuwrzgc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xwtjekxp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3egfciexs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vybqkien.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rxqftxfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wjqkqzyq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dyxiusgj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gpmbsrsa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xbredihq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hhqzbuub.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3sdwdpglw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yslnbfzp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3izclbyoi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mcdvbiiv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kwgmjgtq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrssykyg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wghbsetz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yzatvjxe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ghpudiyg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vcmmjcwz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gtkjtgak.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3lcbachnh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pimmdsfa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ifrceopm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zkbpawos.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ivudpobq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3amvcunsg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wjnmjkxq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cyeyfqkh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gpjhzhbl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xrdpsaqe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jrvmeoua.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3uryayeiz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3drrugyzo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fwqblbbh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idbnofxm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3twevctyr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3loehdovr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qapdpoxh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wydwbabg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hinufdms.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjqleseq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ptqnbkcv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qyjffuid.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oinhhpib.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3twkmmmbn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3siphlsov.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zzccrbof.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3olrqrqvr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kluydkhm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ifvsoush.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nwtfqcik.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3thnvlesc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ebevdqzs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3djwbvuqc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wzjvqgws.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3joeavvtx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mypdlqwx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zpclmkmo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xfibvego.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cmbjgzqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3iqwrjqwy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3clsqhkyu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ixpdbzbh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bclongxh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aupzjckj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3galnjjzx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cmljoglt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ocungijw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqigryt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kbkqxhhq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3etvanaje.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zbcclaur.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hyoszscc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qfnjktbl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ishpymdd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ncansxut.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xkrsnkdi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jgrpugjg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3drgkcxhb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3houzzfsd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nzrcxoaa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mpwdxaeq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xzkptxiy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wwdxnnij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jeconbpm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dyvupsct.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sxmundrv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ogxfcilm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3eexjtnwq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3opumyoqn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3njmjurck.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkignhzk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nedulwao.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nggwbpdn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ubuxakpk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ehdsovje.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3latojueg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zljgnczw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vcvjnzfo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vzzmnkip.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3txtynxpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oiukwaul.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xeeqlegs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wopwzzoq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkacimva.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3opcfhdwv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhyhthmv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tioxvqzi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sygxgjgc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3owkbafbg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3csyltvcz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mnmvfbez.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fvxrporq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vcswuuvr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uipjkpoe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdpjiwoi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3reuirhrv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3urcwnzzh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rwfjxbuv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3llpgicce.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kxedxfzv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hbcatjlr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pknjykry.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nvgltwxj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3svodidsw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztcczsfo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gzlmhrsh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3femlbpet.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3puagrvpe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bdkuxdjt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zyzfezbl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vbdurnqm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dumkroml.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3orzxkays.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3iixtgrzw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fqogvlle.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sprrsatv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kgacavww.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jpfahzkg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3siwyngmo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rixwuurm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rggnhykt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rpcxidnv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rjacmlmj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lhcdsjfj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mrvtwhtz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ktimjcfl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3seklhtxn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nypkasjg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwuyhvuv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xwnfoxzy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ivhsiedn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3posecnwd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cxjegoon.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dcaqpacf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sdaijcby.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3aeybsjrp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ezplkmpm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zuauezld.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wrnwffxd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sqsspoyp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkcvlpgn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ipnkwfwg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jbtekdee.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xonzyite.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ayajluvr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xuhpuvcj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mguxcljx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xnsssjnq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3huplnuer.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rpuvyyht.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rfvwqycu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrgxmnpb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dioniwpp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jdlpetnj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3veyicdga.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pilefqgh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wkrruwhj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3sijjczjc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3domaqvow.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dcgzdwto.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xgvksiyf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3junxttou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3itqcbohz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3waijolsl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3btwxggku.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3puuhfyfd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qkkrlmfe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhbsjmth.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ssbcqrhk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lqgrvopr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oxeaszzq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sjhjynsw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lrqgyzyz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lvwmfohc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xdernpez.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bkobtjje.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwesaajh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wdygkcqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3maozdldh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mupwnyit.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urmfsqfo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ynllmuzg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ixqhntal.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mxssfgvq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rrtkfimt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cxdqmuzt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3arwegsvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cjksegly.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fbhtylof.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iazoeusy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lpjsjekt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vkyuzxkv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ltcrsiwe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3trbokdku.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kvsgauxa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lrmhvuug.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rvhehmfw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3guaxwuqz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fpherycz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kuyhdvej.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hrjricuv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iujaxkzr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xbajmgqd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yanfrtsa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jbfesaug.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xipkrbgt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bmyqeekn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gytlvype.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3iedxnlqo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ihzegojz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjliabvq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nzwqfanc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqbufdbe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ihxhwpbw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ydhkyfci.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sxcytpnh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3arppawwa.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xliwekue.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kxeifuia.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ikjmmdnw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dlvwlcqc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rmomgvpn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jylciljf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zcskwvcy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqltinm.html


<!-- 参考信息 -->
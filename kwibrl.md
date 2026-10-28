代发 wailian999

R. Bash 专题
来源：http://hz.nanxuanxn.top/gtvanfwtms.html

================================================================================
来源：http://hz.cdnleiting.top/gtdduxeeia.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtfaofzlxz.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtvylggvhq.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtclgmlwqn.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtyuiyqyqt.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtktkfbbkn.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gteutxxost.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtwgxbucig.html

[R04] 位置参数
来源：http://hz.sufxvd.cn/gtymtwzpby.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtduvttgws.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtwxawznny.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtbriexiie.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtbxtmxgaf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtohkcaosm.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtiszihevg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ybcxt.top/gtolpxbeie.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtrqdqgpip.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gthagezjtf.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtxlzeiykc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtrrjlfcas.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gttqlsnjpc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gttrymrlwq.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtzvmxrusq.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtnhlefhat.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtvocifeyl.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtfclpiaxd.html

*)     echo "未知命令" ;;
来源：http://hz.ywan-chungtsiang.top/gtlxymbjyi.html

esac
来源：http://hz.tianlin.xyz/gtcznmfykf.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtobwaarzt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtiitrxzry.html

[R13] for 计数循环
来源：http://hz.andypj.xyz/gtiqxzkhrj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtdqidwfqo.html

[R14] C 风格 for
来源：http://hz.wangshuangyany.cn/gtttgebuuy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258.top/gtudxdwycg.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtqzgvxaop.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.birdmap.top/gtrqictnne.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gtfcpqabaj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.smart0.xyz/gtoskohjgf.html

[R17] 数组定义与取值
来源：http://hz.shangyingyoupin.top/gtwpkdsuqc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.quarkkingdee.top/gtseiwuhbv.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gtgixyyzob.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtzsxczjrg.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtbdhwjqtz.html

echo "${#arr[@]}"
来源：http://hz.jinqigfzy.top/gtlhrrjqfg.html

[R20] 关联数组（字典）
来源：http://hz.316326.xyz/gtdkuoxysl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtqunyiqno.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gttzpsynbu.html

echo "${#s}"
来源：http://hz.zycfv.cn/gthfyvpseb.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtaeejfxxe.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtbwspavvj.html

[R23] 字符串替换
来源：http://hz.cucudq.cn/gtafkmepum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj202588.top/gtdqmdexvm.html

[R24] 大小写转换
来源：http://hz.jiagoushi.top/gtzvvucdgv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangshuangyany.cn/gtihwqetjl.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtocqemwrr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtsqrjalbm.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtzvoziyto.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gtcpagndcd.html

[R27] 算术展开
来源：http://hz.hywenlv.cn/gtvdtqcoof.html

echo $((1 + 2 * 3))
来源：http://hz.birdmap.top/gtzoiwpdzc.html

[R28] 浮点运算
来源：http://hz.yanxiufei.cn/gtulkvfjbb.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtzcrivbfl.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtcajilgpn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ywan-chungtsiang.top/gtzrzhxolv.html

[R30] 函数返回状态码
来源：http://hz.yongpay.top/gtbgulmgki.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtesqvumja.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtdlelnvyf.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtiivebtic.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtkyqkmyye.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gotoacloud.top/gtphsfyush.html

[R33] 捕获错误并提示行号
来源：http://hz.yj202588.top/gtdsqtbwoa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ppjwa.cn/gtgmahwqid.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtmvhnxung.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtjgzbwbbv.html

[R35] 后台执行并等待
来源：http://hz.0kj1m.cn/gtegfiqnaz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yanxiufei.cn/gtyygzszvx.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtuukeoocg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhijiandao.cn/gtrgxeonse.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtjsblylxw.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtxhtambaq.html

[R38] 管道串联
来源：http://hz.yvedp.cn/gtyxvhjgzp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtmmdarjon.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtyjvdkosv.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtglzvwtnj.html

[R40] 追加写日志
来源：http://hz.dianchejie.cn/gtuwwjqcyg.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtrjvbzmec.html

[R41] 丢弃输出
来源：http://hz.shangyingyoupin.top/gtujtcxdcb.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtvhthbkfd.html

[R42] 输入重定向
来源：http://hz.wangshuangyany.cn/gtmnsxeacz.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtwkznhajd.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gtuiltlptv.html

find . -name "*.log" -type f
来源：http://hz.kuanghao11.cn/gtowicghyg.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtddeldnvg.html

find . -mtime -7 -type f
来源：http://hz.jlsjyb.cn/gtvyrinjab.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtksjxdzby.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtifomjrms.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtokrvthxm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtuppojxqg.html

[R47] sed 单行替换
来源：http://hz.jyoumei.cn/gtdvpzepnj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gogol.net.cn/gtmfomstbc.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtzedfsbmr.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenzaomai.com/gtjekqcnpw.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtywubayfk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sufxvd.cn/gtjnskxrwb.html

[R50] awk 求和
来源：http://hz.zdqjudy.top/gtslfqpivj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtljmipfjf.html

[R51] 排序去重取前几
来源：http://hz.ppjwa.cn/gtbniujctf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.feifeiyinyue.top/gtkuurvwxm.html

[R52] 统计行数
来源：http://hz.yj20258888.top/gtvfxyvdne.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gthcmdgghf.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtetavpege.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tianlin.xyz/gtskkaibxo.html

[R54] 比较两个文件
来源：http://hz.wangshuangyany.cn/gtchatfynv.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtrzqmbndw.html

[R55] 压缩与解压
来源：http://hz.chenzaomai.com/gttddfgxzr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinyuanbaomall.cn/gtvrfdiojg.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtdwrnegrc.html

scp file user@host:/path/
来源：http://hz.yuxming.cn/gtzeykdhuq.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtdvfkwgwy.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtunvotswb.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtmcmqhnsc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydjk.org.cn/gtneqbpnhz.html

[R59] 发 POST JSON
来源：http://hz.xylfe.cn/gtsldhxpcf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtuqlipxiv.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtavooukqq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtkjqvbabw.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtjzprecdl.html

df -h;  du -sh *
来源：http://hz.cucudq.cn/gtwsqcuqch.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtbutzmmdo.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gteyfzeuzv.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtwllpuzru.html

free -h;  ps aux | grep nginx
来源：http://hz.dashuyun.cn/gtqtotylhd.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtvukmszkx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yvedp.cn/gtivvbogyc.html

[R65] 查看端口占用
来源：http://hz.fzhhl.top/gtnvlhhhxe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtsbbnbgxi.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtymfxldkv.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtywdxlthv.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtzfnmeetz.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtvevcjwop.html

[R68] 计算文件校验值
来源：http://hz.xinyue.icu/gtrnxctwuk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtufinsirg.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtxzyzlkqy.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gtkjvqdmvb.html

[R70] 时间戳与互转
来源：http://hz.yanxiufei.cn/gtzfjmpzes.html

date +%s;  date -d @1700000000
来源：http://hz.cdnleiting.top/gtqdolxhjb.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtzpqigknf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.52xcode.cn/gtdbryqsla.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gttzikuvae.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtvpdmitac.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gthtqcvznd.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gtmbsxuhai.html

[R74] 批量重命名
来源：http://hz.cdnleiting.top/gtrmoazosx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtieglcgvq.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtywwkaale.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtirucjwhp.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtxgooacww.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtjoophoqr.html

[R77] 读取用户输入
来源：http://hz.tanke756.top/gtibnthtgi.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtxvjiqsaj.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtitsunnsm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gtoamuudvn.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtetiefafg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtyuofiyyl.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtdmpvoixp.html

time ./run.sh
来源：http://hz.pengpengdd.cyou/gtxsuvkklu.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqjrkrmbs.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtlqprldnf.html

================================================================================
来源：http://hz.iojbl.cn/gthkxqacew.html

[S01] C：Hello World
来源：http://hz.birdmap.top/gtrqyykawk.html

#include <stdio.h>
来源：http://hz.yj20258.top/gteugqiakr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnxiangtu.top/gtxdznfdjs.html

[S02] C：变量与格式化输出
来源：http://hz.zhixingplan.top/gtqvsejpxl.html

int a = 10; printf("%d\n", a);
来源：http://hz.bjfxy.top/gtdvyefaae.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtaqnchtaj.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtnioupflj.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtrytaxbgf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.svipenyu.cn/gtpkupetqr.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gtmoafketo.html

strlen(s)
来源：http://hz.yangfankeji.com/gtsvpynprm.html

[S06] C：字符串比较
来源：http://hz.ivvv.top/gtxfttqunz.html

strcmp(a, b) == 0
来源：http://hz.316326.xyz/gtzfjboibz.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gtdigavnbc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gtlscnnhwo.html

[S08] C：动态内存分配与释放
来源：http://hz.zycfv.cn/gtlqwkirzx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangkeji.top/gtnriiepmd.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gtnqijustg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtdbjzdgbx.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gthalumlup.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtgxpopezr.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtzusixule.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtvogbvnad.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtxnbprpnh.html

fclose(f);
来源：http://hz.jqgfzy.top/gtjymdsfln.html

[S12] C：写文件
来源：http://hz.chenjidiqi.icu/gtvxkuprgn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xziqi.cn/gtgxgkcxbd.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtjergovdm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yueranfly.top/gtnlskbxds.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtcszglrlu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtfqzneica.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gtjjxraskj.html

(double) a / b
来源：http://hz.dashuyun.cn/gtcadabcog.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtuhrymuoa.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtkfrcpykj.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtmoggnccp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtaagcqhyh.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gttidbgcwt.html

int main(int argc, char **argv)
来源：http://hz.hammf.cn/gtgeyyztyu.html

[S19] C：快速排序
来源：http://hz.hfpthk.cn/gtiygtemqi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtaohcixfe.html

[S20] C：二分查找
来源：http://hz.gzhubu.top/gtkgtzwinr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtwqompfuk.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtmsjjemzb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gtoubusztr.html

[S22] C：字符串转数字
来源：http://hz.hnxiangtu.top/gtnjgyosjx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtxicigtlt.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtyevtkrxo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jlsjyb.cn/gtozqcocmx.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gtdjpiomrx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shuidangran.top/gtrzmptslf.html

[S25] C：内存拷贝
来源：http://hz.yj20258888.top/gtaerlygit.html

memcpy(dst, src, n);
来源：http://hz.yanxiufei.cn/gtisvyrfsn.html

[S26] C：内存清零
来源：http://hz.yueranfly.top/gtaztfplzb.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtsqdkrhlv.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gttejmvtep.html

const double PI = 3.14159;
来源：http://hz.guannengcc.top/gtdgqlecsl.html

[S28] C：静态变量
来源：http://hz.0kj1m.cn/gtfutwibuu.html

static int counter = 0;
来源：http://hz.bjfxy.top/gtvbkopyge.html

[S29] C：变参函数
来源：http://hz.zhaomingkeji.xyz/gttfqhpmky.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj202588.top/gttzpxarbh.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtndtkpwix.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtzwydttqu.html

#define X_H
来源：http://hz.meibo888.top/gteucshuef.html

#endif
来源：http://hz.daria6918.cn/gtburyhypu.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gttbjhjwuj.html

#include <iostream>
来源：http://hz.xuanzx.com/gtrmpfikja.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtzhusqvkw.html

[S32] C++：字符串
来源：http://hz.pycfn.com/gtqsrwbpue.html

std::string s = "hi";  s += "!";
来源：http://hz.tian-w.cn/gtgzlecwiq.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtsnytmheh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhiwuduotai.top/gtvjfkdibz.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtcyiimxfh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhongyouzk.top/gthgmfpvyo.html

[S35] C++：map
来源：http://hz.bjfxy.top/gthmhvpgjg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gthnkvfrqs.html

[S36] C++：unordered_map
来源：http://hz.chenlongwang.top/gtzmbganyl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtgjgfyqjd.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtjzghyich.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinghuilouyu.cn/gtsgamprnj.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtpbsmksgp.html

std::sort(v.begin(), v.end());
来源：http://hz.haohaochexian.top/gtiserwdtw.html

[S39] C++：自定义比较器排序
来源：http://hz.zycfv.cn/gtjhnhmgji.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtfhoxobvd.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtnmhrsdsj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gthubdvrsw.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gtrgadvtfs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.316326.xyz/gtvcnudnny.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtfbigippq.html

class B : public Base { public: void f() override {} };
来源：http://hz.xingfuxueyuan.xyz/gtoqhwzgxk.html

[S43] C++：智能指针
来源：http://hz.shuidangran.top/gtmozjgatx.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangdashe.top/gtpekcpbil.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtnqokpraf.html

void inc(int &x) { ++x; }
来源：http://hz.ydjk.org.cn/gtwziqqcqm.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtdjglbxpb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuetiantiany.cn/gtgrumgacr.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtbtyhsmsg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nwbrower.top/gtyhrbhaiv.html

[S47] C++：结构化绑定遍历
来源：http://hz.jianghu66.top/gtigktwnte.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtyvzhovzq.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtwjtnwiwp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtcpxkklmg.html

while (std::getline(in, line)) { }
来源：http://hz.shzxlz.cn/gthplqczgv.html

[S49] C++：写文件
来源：http://hz.tanke756.top/gtxwdwbhuk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.feifeiyinyue.top/gtorefwyhj.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtkndmfyip.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtucufmndx.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtjyeuousf.html

static_cast<double>(a) / b
来源：http://hz.gaohongyu789.top/gtaxchnsva.html

[S52] C++：const 与 noexcept
来源：http://hz.birdmap.top/gtvogdrevk.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gtsfkserav.html

[S53] C++：移动语义
来源：http://hz.fzhhl.top/gtspxenlue.html

std::vector<int> w = std::move(v);
来源：http://hz.yuanzhike.top/gthfbbhsue.html

[S54] C++：异常处理
来源：http://hz.fengsongda.top/gtemuiebpo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtxsqqjdpb.html

[S55] C++：结构化绑定
来源：http://hz.zhoulong.xyz/gtbfwajieg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zdqjudy.top/gtuxrsjfow.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtgzatjazf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gtejdcxomv.html

[S57] C++：编译期常量
来源：http://hz.cqqwz.cn/gtfyoajdoe.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtaeqbcqka.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtgfhbeuuv.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenjidiqi.icu/gtllsxbiac.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtcssgwbum.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtmpuqpevj.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtdchcpvrm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtrymltyjj.html

================================================================================
来源：http://hz.c1oappe.top/gtrzbwmvfg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gtwcfqmjwl.html

================================================================================
来源：http://hz.xziqi.cn/gteyivzuuy.html


<!-- 参考信息 -->
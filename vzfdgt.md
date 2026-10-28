代发 wailian999

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtmseqdxwq.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtgxhgrfgv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gteldystmn.html

[R05] 参数默认值
来源：http://hz.pycfn.com/gtkqjmywje.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtzfzlyjsf.html

[R06] 判断命令是否存在
来源：http://hz.shzxlz.cn/gtstagsvan.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhoulong.xyz/gtwdurnijb.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtzshtqxlx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtbcynhhlj.html

[R08] 数值比较
来源：http://hz.fengsongda.top/gtedpqdnvi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj202588.top/gtzrcenkgh.html

[R09] 字符串比较
来源：http://hz.jiagoushi.top/gtjuhwvihd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtzbzqrxtb.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtmouvfcws.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtbzrqlwoh.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gttmssphwj.html

case "$1" in
来源：http://hz.shanyushiyangkeji.top/gtbzexsgor.html

start) echo "启动" ;;
来源：http://hz.iojbl.cn/gtywcjvqnh.html

stop)  echo "停止" ;;
来源：http://hz.zdqjudy.top/gteliymkxo.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gtavwanwne.html

esac
来源：http://hz.zhaomingkeji.xyz/gtgvxkzixc.html

[R12] for 遍历文件
来源：http://hz.ehwqpu.com/gtrfduvgrg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sweek.top/gtspuvgivg.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtuopfzjzv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtskmnbztr.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtcjfneinv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtducdipyf.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtlczdmgzq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtgaflangj.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtkzalabur.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtyxvngdet.html

[R17] 数组定义与取值
来源：http://hz.jianghu66.top/gtqiflhamq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtfeseeuoj.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gtmzyzvceu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtquguwxsz.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtaqtypvkf.html

echo "${#arr[@]}"
来源：http://hz.316326.xyz/gthigdfpgv.html

[R20] 关联数组（字典）
来源：http://hz.hammf.cn/gtugawbnyu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.snrcjt.cn/gtylhqcuqg.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gtrnmiynmu.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtowwuaqpy.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtslsqowkp.html

echo "${s:0:5}"
来源：http://hz.zdqjudy.top/gtatpyonqx.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtijabapfg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.0kj1m.cn/gtobcjqxqu.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtfjoxudhb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gtdlyqeyuq.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtdzdffawp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtjbtgegxu.html

[R26] 命令替换
来源：http://hz.zhoulong.xyz/gtrdxzukjn.html

now=$(date +%F); echo "$now"
来源：http://hz.chenlongwang.top/gtjvkoretm.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtswdlabjw.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtlchwbyuo.html

[R28] 浮点运算
来源：http://hz.chenlongwang.top/gtttrurjxh.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtvwaftioj.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtbsptxeud.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.andypj.xyz/gtpiqrpahu.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gttkhyowtp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtuwitvzcm.html

[R31] 局部变量
来源：http://hz.ybcxt.top/gtqkqrpcgg.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtlbpvlwch.html

[R32] 参数个数校验
来源：http://hz.chenjidiqi.icu/gtetuudswz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.9152youxi.cn/gtlcwpwjgf.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gtxiqtegvw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258.top/gtchxhdquq.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gtzihifjdj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtllbohkvj.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtevyobtdo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtybfbwypr.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtdasmwrfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtpokhfggv.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gtiopefuzx.html

files=$(ls -1)
来源：http://hz.gogol.net.cn/gtooswwonr.html

[R38] 管道串联
来源：http://hz.nwbrower.top/gtcfbjeyvs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtfhpwiyhf.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtdcjgxmid.html

cmd > out.log 2>&1
来源：http://hz.xuetiantiany.cn/gtsnkkofgh.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gteobbvhha.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gthqhrtliv.html

[R41] 丢弃输出
来源：http://hz.ppjwa.cn/gtsxzanaju.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtudfuqven.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gtiuvhowku.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtdzwnnvko.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtlmwtyngu.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtixvvczor.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtridzzgyk.html

find . -mtime -7 -type f
来源：http://hz.ywan-chungtsiang.top/gtzrtkonlh.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtfnwljflz.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangkeji.top/gtimmfxojj.html

[R46] 递归替换文件内容
来源：http://hz.ydzc1.top/gtdnrduefa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtecrahcaq.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtdqijbfeo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnxiangtu.top/gtmakkhjxc.html

[R48] awk 取指定列
来源：http://hz.ppjwa.cn/gtqaotcktq.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtomvwvbrq.html

[R49] awk 带条件
来源：http://hz.jiagoushi.top/gtbiugycvx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gtnvtytfrw.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtajruahod.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pengpengdd.cyou/gtcqhizwzg.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtozhykwkl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.havefunace.top/gtjtdahwbd.html

[R52] 统计行数
来源：http://hz.zhengqikj.top/gtdvjkuora.html

wc -l a.txt
来源：http://hz.shuidangran.top/gtricvisdb.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtnvhwfebf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtfcgsrpkx.html

[R54] 比较两个文件
来源：http://hz.sysykeji.top/gtxluivixp.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtpnrcirbb.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtzmqguyyq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydzc1.top/gtoigflllz.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtqicnnkzj.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtaeltnbgw.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtoiekuuuo.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gtuzevkmqt.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtaizqorwh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yvedp.cn/gtvffxtrzl.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtolhdboga.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.quarkkingdee.top/gteeihnnfz.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtbosxsueg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtyixjzhel.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtzggfodvi.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtgfhfxfbx.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtitwixzdt.html

du -ah . | sort -rh | head -10
来源：http://hz.gogol.net.cn/gtkxdbicwq.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtcibijfaj.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtveupnrru.html

[R64] 结束进程
来源：http://hz.zhoulong.xyz/gtaghdkdax.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtnjboklfe.html

[R65] 查看端口占用
来源：http://hz.redwolf501.top/gtocyvorgf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtmotepfjs.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtaeyuhhbl.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gttbwhljkg.html

[R67] 生成随机十六进制串
来源：http://hz.nanxuanxn.top/gtqtlqbyhm.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gthtjkmrpb.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtzkrgblus.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtqivfusrz.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtpkluieix.html

head -c 16 /dev/urandom | base64
来源：http://hz.9152youxi.cn/gtdnygqozr.html

[R70] 时间戳与互转
来源：http://hz.jiagoushi.top/gtodjjezbq.html

date +%s;  date -d @1700000000
来源：http://hz.pycfn.com/gtkhminowi.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gthozrpqjr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtajkjotpe.html

[R72] 等待端口就绪
来源：http://hz.xuanzx.com/gtjhyoaijg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cqqwz.cn/gtcjnopysb.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtoxovyhzm.html

split -l 1000 big.log part_
来源：http://hz.jlsjyb.cn/gtutkqwtky.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtbsbjrovu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gtgegwsbbw.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtgsxdccsx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtfilinkkh.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gtlblcvcus.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtqgwweevo.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gttymnnwxh.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtahybdsks.html

[R78] 交互式菜单
来源：http://hz.zycfv.cn/gtgzoamdxj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dianchejie.cn/gtvgbuvyqn.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtuatqbciz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtpdpxytyo.html

[R80] 查看脚本执行耗时
来源：http://hz.cucudq.cn/gtibcygaok.html

time ./run.sh
来源：http://hz.yuxming.cn/gtpdrghoko.html

================================================================================
来源：http://hz.ehwqpu.com/gtdfkpfelz.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtcmxgdwol.html

================================================================================
来源：http://hz.fzhhl.top/gtfuitihyd.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtfruclgqs.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtkleskcff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtovwgtqff.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtpfootsyc.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtwvnljxqr.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtgtqywvyg.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtmssgebjv.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtemniovjk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.svipenyu.cn/gtfpuepzod.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtmioivjte.html

strlen(s)
来源：http://hz.sxryk.cn/gtopzdienk.html

[S06] C：字符串比较
来源：http://hz.gaohongyu789.top/gtvvklktde.html

strcmp(a, b) == 0
来源：http://hz.hysaishi.cn/gtnecfjilf.html

[S07] C：数组遍历求和
来源：http://hz.yueranfly.top/gtwdikvbnj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtpfgjlyfm.html

[S08] C：动态内存分配与释放
来源：http://hz.chenzaomai.com/gtsjnbixrr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jyoumei.cn/gtkicasgtf.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtkbdeyfwv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnqzz.top/gteqrjefym.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtcguuenyh.html

int *p = &a;  *p = 5;
来源：http://hz.cucudq.cn/gtuwzfuspu.html

[S11] C：逐行读文件
来源：http://hz.haohaochexian.top/gtnrgujkyu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fengsongda.top/gtvxgwbeeo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtakuniehy.html

fclose(f);
来源：http://hz.mhx1999.top/gtcsvealsu.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtyxbziokl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtgxwralbp.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gttkfyzwgd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.52xcode.cn/gtankuefqo.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtgejksifv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gtbbmqffcc.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtorbbmqzu.html

(double) a / b
来源：http://hz.yuanzhike.top/gtkxkfydvd.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gtkwcahbmz.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtdaonaill.html

[S17] C：安全拼接字符串
来源：http://hz.dashuyun.cn/gtsqdshhwh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yvedp.cn/gtswhagmmb.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtmlrcmqlb.html

int main(int argc, char **argv)
来源：http://hz.yueranfly.top/gtddvmsddw.html

[S19] C：快速排序
来源：http://hz.yangfankeji.com/gthwnffjnq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sysykeji.top/gtvsoazero.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gtmqzunurn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtjdevfrkz.html

[S21] C：字符类别判断
来源：http://hz.ivvv.top/gtpshvttsb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtbrekihsb.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtlknsnliz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenzaomai.com/gtuvesugft.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gthmjpzpcf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigfzy.top/gtrtjegazt.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtomgdecac.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtcojryouj.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtkxltbrla.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtmtqlyrrs.html

[S26] C：内存清零
来源：http://hz.aizwys.cn/gtnwyzjmws.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gtvrwocuyd.html

[S27] C：定义常量
来源：http://hz.xinyue.icu/gtxxfrunqx.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtkanpctrt.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtjymubvnx.html

static int counter = 0;
来源：http://hz.tianlin.xyz/gtdkhidpel.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gthbfdsqlv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtqhyzgivd.html

[S30] C：头文件保护
来源：http://hz.tian-w.cn/gtzkojwvsl.html

#ifndef X_H
来源：http://hz.ydzc1.top/gtoejmsccm.html

#define X_H
来源：http://hz.yj202588.top/gtbnwckthv.html

#endif
来源：http://hz.9152youxi.cn/gtgovveewi.html

[S31] C++：Hello World
来源：http://hz.fzhhl.top/gtjxnypbzx.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtnqykxfrk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yanxiufei.cn/gtqdaaiggh.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtelflidlh.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtmuzomtpf.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtaykhcbvf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtsboktpmz.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gthwkyopff.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhiwuduotai.top/gtuojealiu.html

[S35] C++：map
来源：http://hz.gzhubu.top/gtlgbtfpqi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtssqvsuob.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtashxjrxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gttbsiarrt.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtelbrodnq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtrrzevuif.html

[S38] C++：排序
来源：http://hz.tian-w.cn/gtewnhvihm.html

std::sort(v.begin(), v.end());
来源：http://hz.xuetiantiany.cn/gtguhlckwk.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtpdzmaghx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydjk.org.cn/gtteuuejed.html

[S40] C++：查找元素
来源：http://hz.yanxiufei.cn/gthfvfifrd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtgwrjwkmt.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtcvkcbvme.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtijttmmmj.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtyotkpgjr.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtqqmxjpiu.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gtwqvwefyi.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gthhadaqwi.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtxwvuiywu.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtyoygspgm.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtprzaoeon.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtdisxnhml.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtgqzpiosb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gtvysoenyj.html

[S47] C++：结构化绑定遍历
来源：http://hz.vqdsnc.cn/gthetblkhv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xingfuxueyuan.xyz/gtnawqaetx.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gtgftwsmdm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtxyiohafn.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigufen.top/gtceeqndul.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtcxgzbucz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gtdjmxtpdl.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gtxqnhbrub.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.andypj.xyz/gtmhdgoqrf.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtkwocxqca.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtexoqecua.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtawmzieme.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtdpjdbzpn.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtifbntcbf.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtrfplvjoe.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtbacfwttj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.smart0.xyz/gtsfgsrwjm.html

[S55] C++：结构化绑定
来源：http://hz.pengpengdd.cyou/gtcbnpmyic.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangtech.top/gtloljejcx.html

[S56] C++：optional
来源：http://hz.dianchejie.cn/gtswrkifww.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtmynmjptf.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtdrsvangr.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtfruqvfbs.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtbddvovvy.html

namespace ns { int f() { return 1; } }
来源：http://hz.daxiang520.top/gtsjijdafo.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gtgnqgapjq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgfzy.top/gtkgqzthne.html

[S60] C++：遍历并删除元素
来源：http://hz.tanke756.top/gtemmjrknh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtmhubfgpq.html

================================================================================
来源：http://hz.chenlongwang.top/gtpmgmisri.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtntsevnct.html

================================================================================
来源：http://hz.zdqjudy.top/gtvdppbpzw.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gtyfligzie.html

println("Hello")
来源：http://hz.hfpthk.cn/gtshtzmhsl.html

[T02] Kotlin：变量
来源：http://hz.haohaochexian.top/gtyhaqsime.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtcjsackot.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtyqjubgfw.html

"值: $b"
来源：http://hz.jianghu66.top/gtkmzdazkd.html

[T04] Kotlin：空安全
来源：http://hz.snrcjt.cn/gtuytezbby.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtpyxlnras.html


<!-- 参考信息 -->
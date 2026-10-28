代发 wailian999

esac
来源：http://hz.ivvv.top/gtjbklyfhx.html

[R12] for 遍历文件
来源：http://hz.zhixingplan.top/gtdwgekgse.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xinyue.icu/gtzdfhmsjc.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtsdceomxb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtohyoistc.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtglfyhsqc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtemgedsfz.html

[R15] while 逐行读文件
来源：http://hz.andypj.xyz/gttzznkgbd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.smart0.xyz/gtnpmhqtbm.html

[R16] until 等待条件
来源：http://hz.hysaishi.cn/gttkmxwxmf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtgfhqdmkj.html

[R17] 数组定义与取值
来源：http://hz.birdmap.top/gtihlfkvbd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuanzx.com/gtguygkupl.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtvgdqgixe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtlmrkgetl.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtywndsccn.html

echo "${#arr[@]}"
来源：http://hz.jinqigfzy.top/gtkjctliqj.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtyjrbggfk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtawptipbc.html

[R21] 字符串长度
来源：http://hz.bjfxy.top/gtrjedeoqf.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtupfljfiw.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gtkslhustr.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtnqefnoli.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtkuxncnol.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtmobvqcpw.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gthjtdvegf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gthsszglho.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gtjshwfant.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yonumen.top/gtfswbyjwl.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtnbycicoy.html

now=$(date +%F); echo "$now"
来源：http://hz.fzhhl.top/gtljtpimno.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtfodfnzdh.html

echo $((1 + 2 * 3))
来源：http://hz.cucudq.cn/gtjzxcwcqo.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtqzrangyt.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtpbnhmovh.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtgapqgysu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhijiandao.cn/gtydyzftji.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtksaxffft.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtemckmchq.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gtegcekrtq.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhongyouzk.top/gtztcqmctb.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtryvgdrpm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtcdxantbc.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gthvjbmfjs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtbjdshwpn.html

[R34] 退出时清理
来源：http://hz.fzhhl.top/gtqqlaxzsj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtrpfhhcxy.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtblxtiaes.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtcodlgpkk.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtxlopfmvt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.haohaochexian.top/gtmqjhfiul.html

[R37] 把输出赋给变量
来源：http://hz.mhx1999.top/gtxwkyvnpi.html

files=$(ls -1)
来源：http://hz.iojbl.cn/gtroubsqsg.html

[R38] 管道串联
来源：http://hz.zdqjudy.top/gthkhjxgvx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gogol.net.cn/gteublndsb.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtuzvuvbux.html

cmd > out.log 2>&1
来源：http://hz.hammf.cn/gttowluyyz.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtmdvfpouk.html

echo "log" >> out.log
来源：http://hz.jinqigfzy.top/gtktkadxbs.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gttuzqhdjk.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gtfqeknkcv.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gthhwpvjqn.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtlktmerjk.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gtycickdcr.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtmgnesyur.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gttlwxecuz.html

find . -mtime -7 -type f
来源：http://hz.svipenyu.cn/gtdqsqohsf.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtcnbijzmq.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtzbtmvqqv.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtjhyabafn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jianghu66.top/gtzdflqnhc.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtmmfutxeg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtareovtxo.html

[R48] awk 取指定列
来源：http://hz.zhijiandao.cn/gtsqlgdpxp.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtcdzagsnf.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtseufloze.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtzyjmyabe.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gthpsryrrd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtilrmiwee.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gtednrxabe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gthjpugnaa.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtezismshm.html

wc -l a.txt
来源：http://hz.xuanzx.com/gtsmoftmna.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gtxiranbvs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xinyue.icu/gtaozkidvh.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtqyvltvpc.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gtwevtqnbw.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtnkucdmum.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yvedp.cn/gtyuwcdhfu.html

[R56] 远程拷贝
来源：http://hz.shuidangran.top/gtrjwhugbt.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtlqtvgffs.html

[R57] 远程执行命令
来源：http://hz.yanxiufei.cn/gtokuflmed.html

ssh user@host 'uptime'
来源：http://hz.zhijiandao.cn/gtlzfdrduq.html

[R58] 下载文件
来源：http://hz.nanxinkj.top/gtaxpqulcl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hammf.cn/gtdfufcqgu.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtbqcqrptc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gtdghblsfz.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258888.top/gtvfyalwtq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhongyouzk.top/gtkaqehqdg.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtlczcnkqv.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtxmblfbqx.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gthqvpljez.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtletlzepi.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtluauxrgu.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gtfeoggtko.html

[R64] 结束进程
来源：http://hz.zhongyouzk.top/gtwlcixrlh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtjdimnnmt.html

[R65] 查看端口占用
来源：http://hz.52xcode.cn/gtjlsnjymx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gotoacloud.top/gtwlzrtxaf.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtwbunrwfk.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtsdlbmwrq.html

[R67] 生成随机十六进制串
来源：http://hz.meibo888.top/gtjlhxuqrg.html

openssl rand -hex 16
来源：http://hz.sxryk.cn/gtsewedkwz.html

[R68] 计算文件校验值
来源：http://hz.hfpthk.cn/gtihwtidmz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.vqdsnc.cn/gtxlsntttz.html

[R69] 生成随机密码
来源：http://hz.gzhubu.top/gtwjpkkadg.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gtjtopjnjn.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gtvecptwtn.html

date +%s;  date -d @1700000000
来源：http://hz.yongpay.top/gththdpxge.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtlymtmxih.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fzhhl.top/gtejggcdjr.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtopenlowe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gtyzwbjhpv.html

[R73] 分割大日志
来源：http://hz.jinqigfzy.top/gtrmsphlox.html

split -l 1000 big.log part_
来源：http://hz.316326.xyz/gtwjrjqerl.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtmvvdezvv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtbbinelmb.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtpnhlejpu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgufenzy.top/gtszdgifvv.html

[R76] 使用临时文件
来源：http://hz.aizwys.cn/gtzgmnvnfy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtetnoumck.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gttgvfntgx.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtinbwfsam.html

[R78] 交互式菜单
来源：http://hz.c1oappe.top/gttbcvwxsa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xylfe.cn/gtegkprrst.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gtuojzfkwv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guowangkeji.top/gtcklwovot.html

[R80] 查看脚本执行耗时
来源：http://hz.svipenyu.cn/gtdteucfxg.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtyxinnwnt.html

================================================================================
来源：http://hz.cashguo.top/gtkyixueix.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtimuaeyfx.html

================================================================================
来源：http://hz.jyoumei.cn/gtgfhxfnym.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtkwrpmjkm.html

#include <stdio.h>
来源：http://hz.chenlongwang.top/gtwywuqclp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtxpyvbjcz.html

[S02] C：变量与格式化输出
来源：http://hz.zdqjudy.top/gtplngnssm.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gthcbhvstv.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtctubleki.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtbfuhpkgb.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtidkawzfp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258888.top/gtcqwfqwbx.html

[S05] C：字符串长度
来源：http://hz.haohaochexian.top/gtphxfgvfj.html

strlen(s)
来源：http://hz.kuanghao11.cn/gtqqfazbkv.html

[S06] C：字符串比较
来源：http://hz.wangshuangyany.cn/gtqiukgrwp.html

strcmp(a, b) == 0
来源：http://hz.iojbl.cn/gtcjccwnvh.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gtncpqrlci.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.9152youxi.cn/gtbpfhtfgp.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtbrnqlxme.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sysykeji.top/gtmuxvcjfx.html

[S09] C：结构体定义与初始化
来源：http://hz.sxryk.cn/gtnagjjdnk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gtjjdzauus.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtiiczbwcc.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gtykkprfqr.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtimzmvjck.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gttxdvdkia.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtkpdlofmu.html

fclose(f);
来源：http://hz.bjfxy.top/gtiarpmejj.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtksnqfpvg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtevhcqndd.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtcpfuwaeo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gtstoondqj.html

[S14] C：枚举
来源：http://hz.mhx1999.top/gtxvnmxujf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtyofoaefz.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtzqqhxtig.html

(double) a / b
来源：http://hz.hfpthk.cn/gtychzftin.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtehiukyxh.html

x |= (1 << 3);
来源：http://hz.zhixingplan.top/gttflcjbog.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtuxsflvsy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtilxpnhdn.html

[S18] C：命令行参数
来源：http://hz.gzhubu.top/gtionxxbrj.html

int main(int argc, char **argv)
来源：http://hz.cashguo.top/gtkmcmonwv.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtumieggeu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtudbfrmnk.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtuivuhdlc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtdblcnilf.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gttevlriji.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtjtmkmvdg.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtuskitqoo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gttcuzuoli.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtqvtifafb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tanke756.top/gtarswaguw.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtgylqtozp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnqzz.top/gttucuzapo.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtzwmdaqfj.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtkgjbxbqr.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtvgjeytxq.html

memset(a, 0, sizeof a);
来源：http://hz.gzhubu.top/gtohhwjqpd.html

[S27] C：定义常量
来源：http://hz.yangfankeji.com/gtbvlavsnb.html

const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtbdrmatey.html

[S28] C：静态变量
来源：http://hz.andypj.xyz/gtymabresd.html

static int counter = 0;
来源：http://hz.ydzc1.top/gtihxuxikm.html

[S29] C：变参函数
来源：http://hz.tianlin.xyz/gtthidqrxe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gthtxnifki.html

[S30] C：头文件保护
来源：http://hz.chenjidiqi.icu/gttughhxlx.html

#ifndef X_H
来源：http://hz.havefunace.top/gtcvaxcpuk.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gttarktibj.html

#endif
来源：http://hz.yj202588.top/gtmxktufgn.html

[S31] C++：Hello World
来源：http://hz.zycfv.cn/gtxlblkxbm.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtwwltfdma.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cheryme.top/gtvzziyteg.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtzjctotgx.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtmbwrjnwv.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtspggiskx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtivguenev.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtgjdeembu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gtmpkupqel.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtbrgpgnma.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtdsckncpy.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtqckfreqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtuwktbdvv.html

[S37] C++：set
来源：http://hz.birdmap.top/gtwudhdvlg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yonumen.top/gtwehupohs.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtaephiqvc.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gthweqyoun.html

[S39] C++：自定义比较器排序
来源：http://hz.yanxiufei.cn/gttzyuilyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.kuanghao11.cn/gtpaeaiapw.html

[S40] C++：查找元素
来源：http://hz.havefunace.top/gtwavtqqqt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cashguo.top/gtyhhjmqiu.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtmaizfnst.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtcsmesrqn.html

[S42] C++：继承与虚函数
来源：http://hz.jiagoushi.top/gtbgerpzlu.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gtwvgrshxn.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtfpatkvtb.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtidfdpsgb.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtoftrxghv.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtdtdhgxld.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtirkmnuof.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtmychaxnc.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gttqlbswgr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.svipenyu.cn/gtcptoffyv.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydzc1.top/gtfxoudsnc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xziqi.cn/gtyepmsexm.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtpajrnodo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtyelnbflk.html

while (std::getline(in, line)) { }
来源：http://hz.redwolf501.top/gtuetwifqp.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtihkiywta.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtjnbbdobw.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtnnabvnqi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cucudq.cn/gtutdhopao.html

[S51] C++：显式类型转换
来源：http://hz.tianlin.xyz/gtyydkwpvm.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtjdvfojct.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtbbvvtbkk.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtnjhtqqjk.html

[S53] C++：移动语义
来源：http://hz.hfpthk.cn/gtkwbktydi.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtwyifbfxj.html

[S54] C++：异常处理
来源：http://hz.fzhhl.top/gtdxsnbxmm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtyovomxdf.html

[S55] C++：结构化绑定
来源：http://hz.havefunace.top/gtifejgglu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zycfv.cn/gtugtfyawp.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtmnekiuws.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cucudq.cn/gtqfrjuxyp.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtdasjxlrl.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gthhnkrrgu.html

[S58] C++：命名空间
来源：http://hz.zhoulong.xyz/gtsqtttbpj.html

namespace ns { int f() { return 1; } }
来源：http://hz.jlsjyb.cn/gtvollbidy.html

[S59] C++：静态断言
来源：http://hz.shanyushiyangtech.top/gtwwavvtdf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtslcdrpht.html

[S60] C++：遍历并删除元素
来源：http://hz.nwbrower.top/gthmzqvnym.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtvivsikic.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtobvbjxba.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtowcfuugk.html

================================================================================
来源：http://hz.guowangkeji.top/gtkwcbcels.html

[T01] Kotlin：Hello World
来源：http://hz.yuanzhike.top/gtonrvsorh.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtjozwlmiw.html

[T02] Kotlin：变量
来源：http://hz.ydjk.org.cn/gthligzxxf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhijiandao.cn/gtaeqpeyjz.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gtvpuqcgtz.html

"值: $b"
来源：http://hz.fengsongda.top/gtvpjxehol.html

[T04] Kotlin：空安全
来源：http://hz.haohaochexian.top/gthzskubqr.html

val n: String? = null;  n?.length
来源：http://hz.wangdashe.top/gtkkaunxpq.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gthuxbvgxt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtqnhejwfi.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gteodqhwkr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.9152youxi.cn/gtakuuvnoq.html

[T07] Kotlin：集合过滤
来源：http://hz.birdmap.top/gtvahwnxid.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gtqluaiigm.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtfjkybdyv.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtkgpbavle.html

[T09] Kotlin：扩展函数
来源：http://hz.gogol.net.cn/gtmwtiaypd.html

fun String.exclaim() = this + "!"
来源：http://hz.tian-w.cn/gthxaxtgds.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gtnqiazmsk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtlcspdnkx.html

[T11] Kotlin：协程
来源：http://hz.jinqigufen.top/gtawniynup.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hammf.cn/gtwujkchrc.html

[T12] Kotlin：解构声明
来源：http://hz.guowangkeji.top/gtsqwsocwz.html

val (a, b) = Pair(1, 2)
来源：http://hz.9152youxi.cn/gtpsvrqhcn.html

[T13] Kotlin：只读 Map
来源：http://hz.0kj1m.cn/gtlkstqfpy.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtvbgymzyc.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtxgnrameh.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gthxlkugnr.html


<!-- 参考信息 -->
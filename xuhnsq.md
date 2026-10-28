代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtjukkkard.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtjqayemag.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtuelmnwaf.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtkjqcptdi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gtylovxkdr.html

[R16] until 等待条件
来源：http://hz.hnqzz.top/gtqndzvrqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gtlydlxuzn.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gtqggzvcjz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuanzhike.top/gthkempkaj.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtuqlpcsdx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pycfn.com/gtwnmdpnkn.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtxewhmrog.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtsvdtkswg.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtkqvfhfce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jlsjyb.cn/gtizeokhob.html

[R21] 字符串长度
来源：http://hz.feifeiyinyue.top/gtsrohdsbc.html

echo "${#s}"
来源：http://hz.nwbrower.top/gtdplkqmqb.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtxiknyucu.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtbjfrtmxa.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtkrthzhhv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenlongwang.top/gtpbbmggai.html

[R24] 大小写转换
来源：http://hz.dianchejie.cn/gtlukvawhu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gtavcllsqo.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtdncbupoi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xziqi.cn/gtawzfjkuu.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gttlbdtida.html

now=$(date +%F); echo "$now"
来源：http://hz.chenlongwang.top/gtbzchezex.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtuwpbsyrw.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtnczltlxv.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gtxybajlfo.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gtztxhmoar.html

[R29] 定义函数
来源：http://hz.hfpthk.cn/gtcbnxewat.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gtgpyjeijs.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtgsfdtpgj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gtlermsrqw.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtjjfkyufh.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtfileqxkd.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtfflieqfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtalxpfior.html

[R33] 捕获错误并提示行号
来源：http://hz.chenlongwang.top/gtsjtzreah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jlsjyb.cn/gtkgvwamwx.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gtlwdgxsvz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtzchzccdo.html

[R35] 后台执行并等待
来源：http://hz.hnxiangtu.top/gttnxomxyx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtrcvfcqir.html

[R36] 并发执行多个任务
来源：http://hz.ivvv.top/gtaiqnhcnz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenzaomai.com/gtheuaufkp.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtwizfdqqj.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gtgfwvfmcr.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtbbvhbbhi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sweek.top/gtottbkmyo.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtfjlogdoi.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gtgmbqrpnt.html

[R40] 追加写日志
来源：http://hz.yuxming.cn/gtnevesfar.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtcfvlcpdc.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtdmynuida.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtysaihoji.html

[R42] 输入重定向
来源：http://hz.guannengcc.top/gtrnnyekri.html

wc -l < a.txt
来源：http://hz.yonumen.top/gtavunshka.html

[R43] 按名字查找文件
来源：http://hz.zhaomingkeji.xyz/gtpuqamoxp.html

find . -name "*.log" -type f
来源：http://hz.sxryk.cn/gtukdguqnj.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gttwuxuuho.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtihcnoqkz.html

[R45] 批量删除
来源：http://hz.svipenyu.cn/gtshaesekg.html

find . -name "*.tmp" -delete
来源：http://hz.yj202588.top/gtktvnemun.html

[R46] 递归替换文件内容
来源：http://hz.redwolf501.top/gtxbgcqpsi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj202588.top/gtkeaeiehj.html

[R47] sed 单行替换
来源：http://hz.andypj.xyz/gtdmwfgsip.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gtxhdiiayr.html

[R48] awk 取指定列
来源：http://hz.daxiang520.top/gtxjgdnbhn.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtyzahxrff.html

[R49] awk 带条件
来源：http://hz.zycfv.cn/gtgmqtmepc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtjoqeywzi.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtcupjfbty.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtkcswfbta.html

[R51] 排序去重取前几
来源：http://hz.vqdsnc.cn/gtjefrueqx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtomfxrhkv.html

[R52] 统计行数
来源：http://hz.c1oappe.top/gtinhtmgsq.html

wc -l a.txt
来源：http://hz.zhoulong.xyz/gtwcegcizr.html

[R53] 查看文件头与实时尾
来源：http://hz.hnqzz.top/gtqlwganem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gthebwxsao.html

[R54] 比较两个文件
来源：http://hz.gogol.net.cn/gtflwqcaow.html

diff a.txt b.txt
来源：http://hz.ywan-chungtsiang.top/gtlumgcipk.html

[R55] 压缩与解压
来源：http://hz.yanxiufei.cn/gtmcipnisz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtzefspsxv.html

[R56] 远程拷贝
来源：http://hz.xziqi.cn/gtbuflzbpk.html

scp file user@host:/path/
来源：http://hz.xuanzx.com/gtnuunaswr.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtokgehqxq.html

ssh user@host 'uptime'
来源：http://hz.hnxiangtu.top/gtypzegord.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtrrvegxhu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangshuangyany.cn/gtvqagvumg.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gthwlvhtxt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258.top/gtxuxpkqlj.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtstsmqmip.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gthjfbhkyl.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gtpqvsebdw.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gtwginlxsz.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtpljmvmjm.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gtmdkyhvxm.html

[R63] 内存与进程
来源：http://hz.dianchejie.cn/gtnpxbntgr.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtxxqcjoyb.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtywdpojfz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtnyooiant.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gturxiyvov.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtuimvopii.html

[R66] 定时任务
来源：http://hz.zhoulong.xyz/gtbrvnyeui.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtbskdtovx.html

[R67] 生成随机十六进制串
来源：http://hz.tian-w.cn/gttcundwsk.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtuxqljvtr.html

[R68] 计算文件校验值
来源：http://hz.316326.xyz/gtmeoclcny.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xziqi.cn/gtoztzvbmg.html

[R69] 生成随机密码
来源：http://hz.52xcode.cn/gtsvyscwqz.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtfoqfkvil.html

[R70] 时间戳与互转
来源：http://hz.andypj.xyz/gtxcfdgvev.html

date +%s;  date -d @1700000000
来源：http://hz.daria6918.cn/gtqfoiwegr.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtlloxethr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtoiydtkra.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtpaxhmlna.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xingfuxueyuan.xyz/gtjjuqcndz.html

[R73] 分割大日志
来源：http://hz.bjfxy.top/gtreupibgf.html

split -l 1000 big.log part_
来源：http://hz.kuanghao11.cn/gtmtmypoyn.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtulqrbanb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shangyingyoupin.top/gtjldakosg.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gtulekvcti.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dianchejie.cn/gtnylstfui.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gthlvtlxgv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtxzjsyzbm.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gteyidvuyy.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtycbkyweq.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtrzfnrxup.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtynaiahiy.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtrijkyuhy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cashguo.top/gtvzitwkkr.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtqsksnmsj.html

time ./run.sh
来源：http://hz.cqqwz.cn/gtyqldqvmg.html

================================================================================
来源：http://hz.xuanzx.com/gtxdymtqwj.html

S. C / C++ 专题
来源：http://hz.tian-w.cn/gtpwdxobhu.html

================================================================================
来源：http://hz.ydzc1.top/gtxiifxmgg.html

[S01] C：Hello World
来源：http://hz.havefunace.top/gttdekgnkx.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gthcymrmzc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtpcyytfwy.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtyazdfuro.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtgluciaed.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtmtrvceos.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtxibjuoun.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtozqbebdf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtalzjjeck.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gthqbuelyf.html

strlen(s)
来源：http://hz.shangyingyoupin.top/gtvtdqqidh.html

[S06] C：字符串比较
来源：http://hz.meibo888.top/gtpzoppimo.html

strcmp(a, b) == 0
来源：http://hz.zhijiandao.cn/gtouwtcfyu.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtilbbkitn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtoxsadwza.html

[S08] C：动态内存分配与释放
来源：http://hz.yonumen.top/gtemkguhxl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aibaodan.cn/gtcpkhvamm.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gtomciaugg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258.top/gtehjiokzh.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtxtccxcji.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtbvtlhbkl.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtmavwmkau.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gteaobbbck.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gtkvaypxgq.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtmnhhfacm.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtsfsgpgst.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtmriqoplx.html

[S13] C：宏定义
来源：http://hz.svipenyu.cn/gtbevoiveb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangkeji.top/gtwrvnmcmf.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtlcdqotfw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuxming.cn/gtdwrtztiw.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtzolnjblv.html

(double) a / b
来源：http://hz.wangdashe.top/gthlxeyrus.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtbqqswktl.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtmcltjicv.html

[S17] C：安全拼接字符串
来源：http://hz.snrcjt.cn/gtfonwubvb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hysaishi.cn/gtjrydftwn.html

[S18] C：命令行参数
来源：http://hz.yonumen.top/gtjapozsfp.html

int main(int argc, char **argv)
来源：http://hz.yuxming.cn/gtgygjckop.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtxbrrszfz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtdfqwpghf.html

[S20] C：二分查找
来源：http://hz.shanyushiyangkeji.top/gtsvskmksy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gthmtnvohm.html

[S21] C：字符类别判断
来源：http://hz.jqgfzy.top/gtfcdntgzh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtadgqjdxq.html

[S22] C：字符串转数字
来源：http://hz.cqqwz.cn/gtbwcihqrt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxuanxn.top/gtenacdxya.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtaradjfyh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258.top/gthwftcsha.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtyafmpcqj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.snrcjt.cn/gthfwxstnv.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtzbtnhvxy.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtrgaohxnp.html

[S26] C：内存清零
来源：http://hz.yj202588.top/gtrbluyexg.html

memset(a, 0, sizeof a);
来源：http://hz.ehwqpu.com/gtvowbzztl.html

[S27] C：定义常量
来源：http://hz.ehwqpu.com/gtagqbjirp.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtpjssjdae.html

[S28] C：静态变量
来源：http://hz.zhiwuduotai.top/gtvjjpnirj.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtsalzztdr.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtrvcdkowl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xingfuxueyuan.xyz/gtqpixcnjk.html

[S30] C：头文件保护
来源：http://hz.hnxiangtu.top/gtiijxbsgz.html

#ifndef X_H
来源：http://hz.haohaochexian.top/gtclbfypgu.html

#define X_H
来源：http://hz.jqgufenzy.top/gtsmrccata.html

#endif
来源：http://hz.hfpthk.cn/gtkyxcbeuk.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangkeji.top/gtxpaldsli.html

#include <iostream>
来源：http://hz.yvedp.cn/gtxxyqvrmt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ehwqpu.com/gtnbadsgsn.html

[S32] C++：字符串
来源：http://hz.xuetiantiany.cn/gtifginlgm.html

std::string s = "hi";  s += "!";
来源：http://hz.nwbrower.top/gtpbrxbvqx.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gttfhanaaq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtcfufgkch.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtryecolxh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtyvfjvaey.html

[S35] C++：map
来源：http://hz.jinyuanbaomall.cn/gtebfhwzjd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtomhrpbow.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gthuhxeohc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtuxhbjeor.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtoxbgbgmo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtkvbyphqy.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtyypopyve.html

std::sort(v.begin(), v.end());
来源：http://hz.cqqwz.cn/gtyfkqddgj.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtzroenfmq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gtcdfbfiku.html

[S40] C++：查找元素
来源：http://hz.yanxiufei.cn/gtvldfficc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.smart0.xyz/gteikecafg.html

[S41] C++：类与构造函数
来源：http://hz.svipenyu.cn/gtfhjdcdda.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ehwqpu.com/gtipcrtmdm.html

[S42] C++：继承与虚函数
来源：http://hz.mhx1999.top/gtdkqgojhf.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtvybxjcou.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtyyzervkr.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtodpttjph.html

[S44] C++：引用传参
来源：http://hz.jlsjyb.cn/gtnuqevxcj.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtfipicjde.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtxmhsfttp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtgdtvghjw.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtqwyjnrxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hammf.cn/gtmanienso.html

[S47] C++：结构化绑定遍历
来源：http://hz.gzhubu.top/gtgxfdoeyi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtiznirvwj.html

[S48] C++：逐行读文件
来源：http://hz.hywenlv.cn/gtaryzarxu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtitiraqef.html

while (std::getline(in, line)) { }
来源：http://hz.xinyue.icu/gtupxqdfai.html

[S49] C++：写文件
来源：http://hz.snrcjt.cn/gticldzcon.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinyuanbaomall.cn/gtsthgxclb.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gthiooxhss.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtypifupbb.html

[S51] C++：显式类型转换
来源：http://hz.gaohongyu789.top/gtvcmwhwso.html

static_cast<double>(a) / b
来源：http://hz.hongshengwenyu.top/gtudpbiuoh.html

[S52] C++：const 与 noexcept
来源：http://hz.jinghuilouyu.cn/gteeldxcmn.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtivrhtizf.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtlqzdluql.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtxtapvadw.html

[S54] C++：异常处理
来源：http://hz.gzhubu.top/gttinvxrnv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xingfuxueyuan.xyz/gthotugagb.html

[S55] C++：结构化绑定
来源：http://hz.0kj1m.cn/gtlmpblbkg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.bjfxy.top/gtkktjxivk.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtnfgmxkjy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daxiang520.top/gttdrwbiuj.html

[S57] C++：编译期常量
来源：http://hz.jyoumei.cn/gtobamoczz.html

constexpr int N = 10;
来源：http://hz.hfpthk.cn/gtupsohrgz.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtcvptttbt.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhengqikj.top/gtmtdkngbr.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtkekbuudv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangshuangyany.cn/gtgzkcwhdy.html

[S60] C++：遍历并删除元素
来源：http://hz.guowangkeji.top/gtvanjyskv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtrbwkmhwl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlolxivji.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtlninqtjl.html

================================================================================
来源：http://hz.ppjwa.cn/gtijqrkwpm.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gttmdjsjcp.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtgibtyzvm.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtppvhuuxy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtmcqwraov.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtxgkryuaj.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtsvfsuuew.html

[T04] Kotlin：空安全
来源：http://hz.jinqigfzy.top/gtdvyfzouk.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtgmvomrrq.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gtxujxpijl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtnzikawaa.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtfpdtbrhm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtkherhuyp.html

[T07] Kotlin：集合过滤
来源：http://hz.yuxming.cn/gtrbrivtmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tanke756.top/gtzlrkiowi.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtbrbtlgto.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gttffvwuas.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtkbyevpac.html

fun String.exclaim() = this + "!"
来源：http://hz.quarkkingdee.top/gtjmsdtgst.html

[T10] Kotlin：默认参数
来源：http://hz.gogol.net.cn/gtqxynbped.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtkhjwnhog.html

[T11] Kotlin：协程
来源：http://hz.shangyingyoupin.top/gtmweqvrjh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gtvhowfgol.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtepfodsja.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gttadzegbc.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtbapmgqmc.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gtirqwdyzb.html

[T14] Kotlin：循环
来源：http://hz.dianchejie.cn/gtaajjtkuv.html

for (i in 1..10) println(i)
来源：http://hz.gogol.net.cn/gtxgurxaqk.html

[T15] Kotlin：接口
来源：http://hz.xziqi.cn/gtsyhdsfvv.html

interface Shape { fun area(): Double }
来源：http://hz.gogol.net.cn/gtxlcfaddw.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtmboyyucn.html

print("Hello")
来源：http://hz.xziqi.cn/gtjdtbjbbq.html


<!-- 参考信息 -->
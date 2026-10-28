代发 wailian999

esac
来源：http://hz.feifeiyinyue.top/gtupyzjqaa.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtkwchkais.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gtjmnmzckb.html

[R13] for 计数循环
来源：http://hz.xuetiantiany.cn/gtqayjetpy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenzaomai.com/gtizvooqvp.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtgarjppva.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tianlin.xyz/gtsczvwtmu.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gttxntqkmy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtbrpwxjcu.html

[R16] until 等待条件
来源：http://hz.hywenlv.cn/gtqrmjdnzb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gtntwkjzzc.html

[R17] 数组定义与取值
来源：http://hz.hysaishi.cn/gttaumohsq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtttrkqbza.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtelqloxjd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ivvv.top/gtjlsqfrgf.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtxkxfuvhe.html

echo "${#arr[@]}"
来源：http://hz.tanke756.top/gtmslohvny.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtzblokfhm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtntlfwzph.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtdajqftfz.html

echo "${#s}"
来源：http://hz.sxryk.cn/gttjhnlfjz.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtfdrsyjkf.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtubkcrqzd.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtrwgkstju.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtebnflsad.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtbztoyotf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtmtdzufow.html

[R25] 去后缀 / 去前缀
来源：http://hz.tanke756.top/gtoebhmzph.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gogol.net.cn/gtizoiemuj.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtynwtgzrh.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtjafwvsih.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtdkayhugt.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtbxvwfzpb.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtzgjdzjyn.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnqzz.top/gtyoxlgdba.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtlrbqludz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.meibo888.top/gtartdlzjs.html

[R30] 函数返回状态码
来源：http://hz.yj202588.top/gthmsrwzvd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gtfqprxgds.html

[R31] 局部变量
来源：http://hz.vqdsnc.cn/gtgzzztjhv.html

f() { local x=1; echo "$x"; }
来源：http://hz.jyoumei.cn/gtqptuqear.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtywmnusss.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nwbrower.top/gtfysxvrjh.html

[R33] 捕获错误并提示行号
来源：http://hz.xylfe.cn/gteqabufkl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtjjrwqfff.html

[R34] 退出时清理
来源：http://hz.ehwqpu.com/gtbufregbs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gteujtohsr.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtorxbdamv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dianchejie.cn/gtxtqovzxg.html

[R36] 并发执行多个任务
来源：http://hz.cdnleiting.top/gtwffwcajn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtkoawuhhs.html

[R37] 把输出赋给变量
来源：http://hz.zhongyouzk.top/gtygksdlgl.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtnqvhvfkj.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtozxuzfbp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtbguvlyts.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gthuntywct.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gteqkmppyq.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gteuyzsfrt.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtubrmffem.html

[R41] 丢弃输出
来源：http://hz.ywan-chungtsiang.top/gtwbergyzn.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtsymrdszw.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gthtjvtdfw.html

wc -l < a.txt
来源：http://hz.sweek.top/gtagcklzjg.html

[R43] 按名字查找文件
来源：http://hz.hywenlv.cn/gtmyxamypf.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtqjphnbit.html

[R44] 按修改时间查找
来源：http://hz.zhongyouzk.top/gtmatehiap.html

find . -mtime -7 -type f
来源：http://hz.yueranfly.top/gtyxubimtt.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtpqplldpo.html

find . -name "*.tmp" -delete
来源：http://hz.zdqjudy.top/gtpjwryiav.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gtazqbksob.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dianchejie.cn/gtttnzggnr.html

[R47] sed 单行替换
来源：http://hz.pycfn.com/gtebjyvxrt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhongyouzk.top/gtaxmkgdzx.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gteojzkfzq.html

awk '{print $1, $3}' a.txt
来源：http://hz.sxryk.cn/gtambrunpx.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtsbnukhol.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gttsuqspwj.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtprjrjqbf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtrhvdtjny.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gtpkmhvbws.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtqdloylda.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtkvfyfift.html

wc -l a.txt
来源：http://hz.andypj.xyz/gtxpexxlpq.html

[R53] 查看文件头与实时尾
来源：http://hz.zhiwuduotai.top/gtwgqbewqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtricrkoeb.html

[R54] 比较两个文件
来源：http://hz.haohaochexian.top/gtcvtejbgx.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtfxauefpb.html

[R55] 压缩与解压
来源：http://hz.ppjwa.cn/gtyrnhkuza.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtytpczcte.html

[R56] 远程拷贝
来源：http://hz.yj20258.top/gtlqvdsdwo.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtxvtnidur.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtyubnpfec.html

ssh user@host 'uptime'
来源：http://hz.quarkkingdee.top/gtlyenmbiz.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtgjqtffvj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gtygcavqjs.html

[R59] 发 POST JSON
来源：http://hz.jqgfzy.top/gtphqnhwej.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sxryk.cn/gtiyxmsalu.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtzfxxpwgq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtezefcogf.html

[R61] 磁盘占用
来源：http://hz.316326.xyz/gtlgcxhffo.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gtouqjxacj.html

[R62] 找最占空间的文件
来源：http://hz.52xcode.cn/gtjuagtqpo.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtwgphgujf.html

[R63] 内存与进程
来源：http://hz.yueranfly.top/gtuwxdtfzo.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtffmzmdey.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtlkeepwjp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgufenzy.top/gtsdhinyas.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtmbbmvnqy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtiepobobq.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gthbymsjdy.html

crontab -e;  crontab -l
来源：http://hz.xziqi.cn/gtnobsihrg.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigfzy.top/gthnskityr.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtmhviupis.html

[R68] 计算文件校验值
来源：http://hz.cashguo.top/gtlnktykhe.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jlsjyb.cn/gtahybjwit.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gthqnxyize.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtpdxiekyh.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtpdihlbnv.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtabrjlkay.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtadvteotd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtedzhbwaq.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gttsbjlwtz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtimrvnteq.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gthlnqpukh.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gthprpnoes.html

[R74] 批量重命名
来源：http://hz.meibo888.top/gtsjjrxztk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gttuoycnsz.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gtxezcpwjn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ybcxt.top/gtriwziogg.html

[R76] 使用临时文件
来源：http://hz.smart0.xyz/gtqcojpwyg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtkxdifeoe.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtbrnlmxpv.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtygsbimlu.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtzbzfrhcq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258.top/gtypmbiivd.html

[R79] 解析命令行选项
来源：http://hz.meibo888.top/gtkzspyvuh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnxiangtu.top/gtfnthctsg.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gtvlqkjakm.html

time ./run.sh
来源：http://hz.mhx1999.top/gtmcyrlyii.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtffyvimkq.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtenhndewm.html

================================================================================
来源：http://hz.bjfxy.top/gtkqxbmfow.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtlwpkvcqc.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gtyqtntasa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtdjqwnkuj.html

[S02] C：变量与格式化输出
来源：http://hz.yueranfly.top/gtzqdxhzqv.html

int a = 10; printf("%d\n", a);
来源：http://hz.pycfn.com/gtrkdwxgwg.html

[S03] C：读入整数
来源：http://hz.iojbl.cn/gtraealtvz.html

int x; scanf("%d", &x);
来源：http://hz.gaohongyu789.top/gtdkmqwljo.html

[S04] C：字符串复制
来源：http://hz.jiagoushi.top/gtotecfuqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dianchejie.cn/gtspshymux.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtewlgknis.html

strlen(s)
来源：http://hz.yj202588.top/gtoxlfecfo.html

[S06] C：字符串比较
来源：http://hz.ydjk.org.cn/gtmwlrbxzd.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtdplyphgo.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtrxbaztuk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gtaulvkfhd.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtmruoczod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtqghcoysz.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gtppugkmyq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pengpengdd.cyou/gtkebqrsrg.html

[S10] C：指针与解引用
来源：http://hz.c1oappe.top/gtdqnsjlke.html

int *p = &a;  *p = 5;
来源：http://hz.guowangkeji.top/gtedzfnvbq.html

[S11] C：逐行读文件
来源：http://hz.gaohongyu789.top/gtnulxkpys.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtwxoleqbr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tian-w.cn/gtnzbiicbb.html

fclose(f);
来源：http://hz.yvedp.cn/gtwwudpoxs.html

[S12] C：写文件
来源：http://hz.chenzaomai.com/gtzfmjtzsh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtbbykpxhr.html

[S13] C：宏定义
来源：http://hz.tanke756.top/gtdugedmkt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gtsqtlomnv.html

[S14] C：枚举
来源：http://hz.zhiwuduotai.top/gtwsafklbv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtynagakhw.html

[S15] C：类型转换
来源：http://hz.smart0.xyz/gtxyhdrusg.html

(double) a / b
来源：http://hz.dianchejie.cn/gtqgwdgamf.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtnrecrozj.html

x |= (1 << 3);
来源：http://hz.birdmap.top/gtpqpnsxpn.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtxbdsoenz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtaqugppqw.html

[S18] C：命令行参数
来源：http://hz.daria6918.cn/gtvzjjnrlv.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtpxazbprd.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gtzxcrvpyw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtyudkdqhd.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtwwpaofzo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtjsfznrmn.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtlzfxyznw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sweek.top/gtrobjdmhw.html

[S22] C：字符串转数字
来源：http://hz.jinghuilouyu.cn/gtbezixvmj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gticmzrjtk.html

[S23] C：随机数
来源：http://hz.tianlin.xyz/gtntzftfhh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ybcxt.top/gtthdjgiix.html

[S24] C：获取本地时间
来源：http://hz.redwolf501.top/gtsvscjbdp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xylfe.cn/gtzzhnhhco.html

[S25] C：内存拷贝
来源：http://hz.jinqigfzy.top/gttpglgjzx.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtvfzxngzh.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gtgsltvtib.html

memset(a, 0, sizeof a);
来源：http://hz.yongpay.top/gtlwzlereg.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gtuuynmfrv.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtvadwpyvi.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtklqjnyrg.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtiwtebsyc.html

[S29] C：变参函数
来源：http://hz.aizwys.cn/gtxqjjivet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hfpthk.cn/gtbrbgaxfu.html

[S30] C：头文件保护
来源：http://hz.sxryk.cn/gtmvhilznz.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtfzcxvndh.html

#define X_H
来源：http://hz.yj20258.top/gtwdbuutoo.html

#endif
来源：http://hz.tian-w.cn/gtzuslhbuv.html

[S31] C++：Hello World
来源：http://hz.hnxiangtu.top/gtrpaqlksz.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gthkxikmgv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtpvykbwle.html

[S32] C++：字符串
来源：http://hz.jiagoushi.top/gthqpmrnxs.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtmixdkhjp.html

[S33] C++：vector 增删
来源：http://hz.hammf.cn/gthxwydvmr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtxyymjizh.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtptomdnym.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtdcvicgek.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtsaorpcaw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtexyxsqyt.html

[S36] C++：unordered_map
来源：http://hz.xuetiantiany.cn/gtmjhrucms.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtdxrmjkkm.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtanfnergi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhixingplan.top/gtdseplegh.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtfgbhombk.html

std::sort(v.begin(), v.end());
来源：http://hz.zycfv.cn/gthmjqgfkx.html

[S39] C++：自定义比较器排序
来源：http://hz.zhaomingkeji.xyz/gtqqmslbox.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtoelkqtuk.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtcpzqwnlp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtoxmicxas.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtoccrfvet.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtwbvkopce.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtqzufqazx.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gtbpujckqa.html

[S43] C++：智能指针
来源：http://hz.daria6918.cn/gtpmvrehqs.html

auto p = std::make_unique<int>(5);
来源：http://hz.sysykeji.top/gtkeiqojln.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gthtclsdbc.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtzlueexdn.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtnbwfozne.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gteailhusi.html

[S46] C++：函数模板
来源：http://hz.yueranfly.top/gtapglkwdu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtadzybgft.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtiyxjthrh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtspsdiknc.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gtahpddexj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zdqjudy.top/gtwdzhvbfl.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtqtynrgth.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtmbzewywd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtntwudace.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gthgckqszq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhengqikj.top/gtvcrcbxnm.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtnvhdbaky.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtaoojthyf.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtejpqjcik.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtowewybxi.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtpyhbgrpp.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtmhujqgak.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gtaznnujhv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gaohongyu789.top/gthfhubkgz.html

[S55] C++：结构化绑定
来源：http://hz.pengpengdd.cyou/gtervokrck.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gttnymfmrk.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtgcgapuns.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gthfafjsgl.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtfiofgles.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gthlyhrgmn.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtgltzybjo.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtnvgkdiyx.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtvmwjbzfa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtdjadifdg.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gtlvbbhesp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtjimrizjc.html

================================================================================
来源：http://hz.nwbrower.top/gtslgiavdj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtwdknqvge.html

================================================================================
来源：http://hz.yongpay.top/gtwjcuihim.html

[T01] Kotlin：Hello World
来源：http://hz.jinqigfzy.top/gthssxclij.html

println("Hello")
来源：http://hz.yonumen.top/gtosyrwday.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtbhmvtrlq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hammf.cn/gttpjltqus.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangkeji.top/gthfhqvsif.html

"值: $b"
来源：http://hz.guowangkeji.top/gtbbnrcwkw.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtvqhpbedo.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtgalhxmvx.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtnpjovenb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtlwzqzokv.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtqiogxaro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtriloxbyw.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtuhixntoj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtfoiqpnrm.html

[T08] Kotlin：数据类
来源：http://hz.ivvv.top/gtidmqeosf.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtidtuqzdb.html

[T09] Kotlin：扩展函数
来源：http://hz.shangyingyoupin.top/gtbtttvjbi.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtleepatyt.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gteqabqegl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dashuyun.cn/gtwbdsjtwo.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtmfubjhfq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtjjzyrwer.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigfzy.top/gtysxchnzh.html

val (a, b) = Pair(1, 2)
来源：http://hz.hongshengwenyu.top/gtbcuuxbok.html

[T13] Kotlin：只读 Map
来源：http://hz.nwbrower.top/gtgjuvalqg.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gtmpschcqq.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtadfdiret.html

for (i in 1..10) println(i)
来源：http://hz.yongpay.top/gtybcbueqw.html


<!-- 参考信息 -->
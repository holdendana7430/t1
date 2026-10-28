代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.guannengcc.top/gtnntpoyxx.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtcujeofzi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtcvugafji.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtphsmmihy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtenzqgwpi.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtlwbuvdht.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hysaishi.cn/gtmuqrxprk.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtckfvodwm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtuvmaxwko.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gtkebruebw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sufxvd.cn/gtbgszbxds.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gtwlqykncc.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtbcdvrquo.html

[R20] 关联数组（字典）
来源：http://hz.guowangkeji.top/gtbvbfixse.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtmqfktaju.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gtixcsqbmt.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtizwbuuzb.html

[R22] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtotqxpozr.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gtmetdrdgl.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtmdjlwsxh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtwkixvbtj.html

[R24] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtcjaocnpo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yvedp.cn/gtqvwjknxe.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtgauvzjva.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.feifeiyinyue.top/gtxpeentji.html

[R26] 命令替换
来源：http://hz.gotoacloud.top/gtkymbsota.html

now=$(date +%F); echo "$now"
来源：http://hz.ybcxt.top/gtlqsvjdut.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtascdmgfg.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtndibqgip.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtiktzfuwn.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtdihczafk.html

[R29] 定义函数
来源：http://hz.smart0.xyz/gtnjyyafym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gtfxrhpunc.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtnyuhrnai.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gttmvpfvtu.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtqjfpwzbi.html

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gtzmnvlxny.html

[R32] 参数个数校验
来源：http://hz.mhx1999.top/gtohdkfjyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtdjxuxhhr.html

[R33] 捕获错误并提示行号
来源：http://hz.yuanzhike.top/gtjzugsqbo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ybcxt.top/gtdbosasfn.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtjifugjub.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gttbltnkdu.html

[R35] 后台执行并等待
来源：http://hz.shuidangran.top/gtycrpxzkh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtdereufom.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gtfofqcspd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuetiantiany.cn/gtmukutvbs.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtkdecllyf.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtwpraeiic.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtuwpcdvem.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtmqdilvaa.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gtaxungskl.html

cmd > out.log 2>&1
来源：http://hz.yj20258.top/gtkjnlmcme.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtwarrjrnb.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtjhvssbop.html

[R41] 丢弃输出
来源：http://hz.jqgufenzy.top/gtnqaqlwix.html

cmd >/dev/null 2>&1
来源：http://hz.redwolf501.top/gttzushynn.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtchdypllu.html

wc -l < a.txt
来源：http://hz.shzxlz.cn/gttufrkynd.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtuqnttckx.html

find . -name "*.log" -type f
来源：http://hz.cdnleiting.top/gtbqqrchmr.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtkxhufvsa.html

find . -mtime -7 -type f
来源：http://hz.cashguo.top/gtcjyclacc.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtoyowdssv.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtuyrlevzn.html

[R46] 递归替换文件内容
来源：http://hz.cashguo.top/gthqywxwgb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtfyhfqmac.html

[R47] sed 单行替换
来源：http://hz.quarkkingdee.top/gtvvvofxwp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gtlgbcsxjy.html

[R48] awk 取指定列
来源：http://hz.0kj1m.cn/gtoonydbeh.html

awk '{print $1, $3}' a.txt
来源：http://hz.tianlin.xyz/gtzsfnlfnd.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtmtvdbmwg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.vqdsnc.cn/gtebbgtmhh.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtjyhwmkrj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtgeuxhkow.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtxhbijzgz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtcarykcht.html

[R52] 统计行数
来源：http://hz.nwbrower.top/gtvnafbjlh.html

wc -l a.txt
来源：http://hz.yueranfly.top/gtqshldlag.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtsfrfbxwc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtnjaevpmw.html

[R54] 比较两个文件
来源：http://hz.jinghuilouyu.cn/gtfrszhcsh.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtevmkjwzu.html

[R55] 压缩与解压
来源：http://hz.svipenyu.cn/gtlbrqcepl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gtfkawvszd.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gtbginivrx.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gthtljsopg.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtrhnzptbt.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtotcupsfe.html

[R58] 下载文件
来源：http://hz.nwbrower.top/gtzsfvlifp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gttkrqupsx.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtlftkwkjx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gthrkypdhh.html

[R60] 只看 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtwgmffcqz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gtrookbnyl.html

[R61] 磁盘占用
来源：http://hz.chenzaomai.com/gtegmrjrqz.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gtbahdrfbj.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtwoqjxsqj.html

du -ah . | sort -rh | head -10
来源：http://hz.wangdashe.top/gtpyzzqpiv.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtoisucdsa.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtjetyjjbr.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtzvnkswnz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtoddkvcnk.html

[R65] 查看端口占用
来源：http://hz.zhengqikj.top/gtwkkunths.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.havefunace.top/gtunarcefo.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtzvuehxah.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtueckpifa.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtrhydhdol.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtsphccxcd.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtntmenlnr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtbohrtjsn.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gthzbmfrxy.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxinkj.top/gthqzgyodb.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtluttqgrl.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gtbbgovgas.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtqcswzldg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtinadlcyv.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtelxmpfll.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtulqyhhzy.html

[R73] 分割大日志
来源：http://hz.jiagoushi.top/gtvpodnhll.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtesejoxgr.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gtqyedoxdi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daxiang520.top/gtpznybgky.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtwezzxnat.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guowangkeji.top/gtrzhxwpfp.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtergihrfg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtgvktrotn.html

[R77] 读取用户输入
来源：http://hz.tian-w.cn/gtilqmpspb.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtjvfbdvrj.html

[R78] 交互式菜单
来源：http://hz.snrcjt.cn/gtdldnkxyo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtqqpggxzp.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtiajpjoom.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xylfe.cn/gtrpqmtlxh.html

[R80] 查看脚本执行耗时
来源：http://hz.zhoulong.xyz/gtvysconjl.html

time ./run.sh
来源：http://hz.birdmap.top/gtffbvrohp.html

================================================================================
来源：http://hz.yueranfly.top/gtwdtyydwf.html

S. C / C++ 专题
来源：http://hz.hnxiangtu.top/gtpdhhojdj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtytyjxuna.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtigtqfnns.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtxpinorgc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnxiangtu.top/gtgjmbmgww.html

[S02] C：变量与格式化输出
来源：http://hz.jqgfzy.top/gtrsgnmfro.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtxizuhmpf.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtgucqgixt.html

int x; scanf("%d", &x);
来源：http://hz.guannengcc.top/gtewpeserg.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gttnalrelj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtdzzdvxal.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gtbhrcvkam.html

strlen(s)
来源：http://hz.sysykeji.top/gtdnzpfxkb.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gtdehkgpui.html

strcmp(a, b) == 0
来源：http://hz.yj202588.top/gtwxefvpvp.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtimqzctpz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtrionjwym.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtbpuovvjn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtqjzcrwhj.html

[S09] C：结构体定义与初始化
来源：http://hz.shangyingyoupin.top/gtseiqczjv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gtfbegkuji.html

[S10] C：指针与解引用
来源：http://hz.chenlongwang.top/gtdnluvxpa.html

int *p = &a;  *p = 5;
来源：http://hz.ywan-chungtsiang.top/gtjqlrjhbk.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gtltntkckz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtzvewyqii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gtgxlkrkxs.html

fclose(f);
来源：http://hz.hongshengwenyu.top/gtwgfgyyfd.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtuxskztee.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aizwys.cn/gtphxnaycf.html

[S13] C：宏定义
来源：http://hz.tanke756.top/gtrlodneog.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yangfankeji.com/gtezrhdbxw.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gtnufthnmc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.andypj.xyz/gtduznncur.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtevdwmgss.html

(double) a / b
来源：http://hz.andypj.xyz/gtupiqmrri.html

[S16] C：位操作置位
来源：http://hz.shuidangran.top/gtlhppayga.html

x |= (1 << 3);
来源：http://hz.zhengqikj.top/gtljvzkaen.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtbtvrwngn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cucudq.cn/gtbdovwnsf.html

[S18] C：命令行参数
来源：http://hz.cheryme.top/gtkfqkydeu.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtnkdqxltg.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtiuwecevk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gttcmsgrhl.html

[S20] C：二分查找
来源：http://hz.ivvv.top/gtspahyzne.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtqmuicpmq.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtdpdooxym.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtjgdnndvv.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtutjncgoe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtaslxqaaf.html

[S23] C：随机数
来源：http://hz.aizwys.cn/gtvpofiyfu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtyynfbovq.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtakogvgzj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtdhjsztud.html

[S25] C：内存拷贝
来源：http://hz.yvedp.cn/gtmozbjptu.html

memcpy(dst, src, n);
来源：http://hz.jyoumei.cn/gtvftsdqua.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtnboxwilp.html

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gtcgwsemkv.html

[S27] C：定义常量
来源：http://hz.redwolf501.top/gtuzqtprhn.html

const double PI = 3.14159;
来源：http://hz.ybcxt.top/gtvbaftorb.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtknpytosv.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtybnnvjkv.html

[S29] C：变参函数
来源：http://hz.pycfn.com/gttrvmzmoi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yvedp.cn/gtoxpkzuud.html

[S30] C：头文件保护
来源：http://hz.smart0.xyz/gtagdgwnkp.html

#ifndef X_H
来源：http://hz.hysaishi.cn/gtfgywnwcp.html

#define X_H
来源：http://hz.ppjwa.cn/gtugzevoux.html

#endif
来源：http://hz.daria6918.cn/gtxgsfcish.html

[S31] C++：Hello World
来源：http://hz.wangdashe.top/gtnopzvxqn.html

#include <iostream>
来源：http://hz.ivvv.top/gteyotrsuj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shzxlz.cn/gtzbakyobd.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtomdrbqew.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtcwyjcvyz.html

[S33] C++：vector 增删
来源：http://hz.zycfv.cn/gtrmjgsdec.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guowangkeji.top/gtjvhyvcbv.html

[S34] C++：遍历 vector
来源：http://hz.zhixingplan.top/gtemogqiam.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ybcxt.top/gtnbszjaig.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtyzgbmtxy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtccazgzsm.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtfytbqnbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtkjsjgdvs.html

[S37] C++：set
来源：http://hz.pycfn.com/gtaokkpjbt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xziqi.cn/gtqtonabiv.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtphmxwjdq.html

std::sort(v.begin(), v.end());
来源：http://hz.chenjidiqi.icu/gtbkmqoxti.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtrikwmduf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhixingplan.top/gtvdddxxuq.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtseusvoyz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtntfrjlxi.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gtwgylexnb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gtligxnpsb.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtjnuxghty.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gtjwxifrzq.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gtrcphrygt.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinghuilouyu.cn/gtbrplldpe.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtybhfbhhi.html

void inc(int &x) { ++x; }
来源：http://hz.yj202588.top/gtbpnnousl.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtczujsfgv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dianchejie.cn/gtllovfvju.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtaihacajl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtgeqafuja.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtgzlwxmdj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtkhskkwwq.html

[S48] C++：逐行读文件
来源：http://hz.xuetiantiany.cn/gtfsmxeyds.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtjpkcqgph.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gtwbgywqcu.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtxcxiuodx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuanzx.com/gtnzcyexxh.html

[S50] C++：格式化数字
来源：http://hz.hammf.cn/gtcsosicnm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.kuanghao11.cn/gtwhwloucr.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtpinuskqu.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtckoctjct.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gtapsyujio.html

int size() const noexcept { return n_; }
来源：http://hz.xylfe.cn/gtwmhvyhbe.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtqcsdrxbj.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtjrdknftn.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtxclqeehx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtouodkquo.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtbrlvltlw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinyuanbaomall.cn/gtczhkhbuh.html

[S56] C++：optional
来源：http://hz.meibo888.top/gtbfwzbiko.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtgejhscfo.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtprzykbhk.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtljqxholm.html

[S58] C++：命名空间
来源：http://hz.ehwqpu.com/gtfbdzulbo.html

namespace ns { int f() { return 1; } }
来源：http://hz.daxiang520.top/gttwilqfak.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtcqveegei.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtaspqhdis.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtesgsxjne.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhoulong.xyz/gtkprmyzdv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzemmzsud.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtyemhtxrx.html

================================================================================
来源：http://hz.xziqi.cn/gthmqpnxsg.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtvoysczaj.html

println("Hello")
来源：http://hz.iojbl.cn/gtticymryg.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtjyrkposi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.birdmap.top/gtbuamshjx.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxinkj.top/gtfkagleaj.html

"值: $b"
来源：http://hz.jiagoushi.top/gtdcokyndr.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtvwfjrduq.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtcwbxhutp.html

[T05] Kotlin：when 表达式
来源：http://hz.zhiwuduotai.top/gtpcnfvqrb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hysaishi.cn/gtwlcfvoxe.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtvlgzqbey.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtclezsldq.html

[T07] Kotlin：集合过滤
来源：http://hz.chenlongwang.top/gtpllllbrz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yanxiufei.cn/gtituzjjxv.html

[T08] Kotlin：数据类
来源：http://hz.jlsjyb.cn/gthnaetydi.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gthcigziuz.html

[T09] Kotlin：扩展函数
来源：http://hz.bjfxy.top/gtwxeljtfa.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtxqbkwiyh.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtwbypyccx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guowangkeji.top/gtdutruoil.html

[T11] Kotlin：协程
来源：http://hz.smart0.xyz/gtspeuuiyb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hysaishi.cn/gtgtzqivwe.html

[T12] Kotlin：解构声明
来源：http://hz.chenzaomai.com/gttpsivvvx.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gthzjjooat.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtfpxrratt.html

val m = mapOf("a" to 1)
来源：http://hz.xuetiantiany.cn/gtehhtwayn.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtvsamdvjy.html

for (i in 1..10) println(i)
来源：http://hz.ydzc1.top/gtvdigmfje.html

[T15] Kotlin：接口
来源：http://hz.xuanzx.com/gttpejoftu.html

interface Shape { fun area(): Double }
来源：http://hz.pengpengdd.cyou/gtzvxgyzir.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtfxiaxjhi.html

print("Hello")
来源：http://hz.sxryk.cn/gtppjnicgp.html


<!-- 参考信息 -->
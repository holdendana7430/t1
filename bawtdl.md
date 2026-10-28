代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.hongshengwenyu.top/gtjlxrewby.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigufen.top/gtyvulxdgm.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtqrfjauhb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtqevujivx.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtwgiwvmnw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dianchejie.cn/gtmujtobsn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gogol.net.cn/gtlavvqpsd.html

[Q89] 判断表是否存在
来源：http://hz.cheryme.top/gtvxrjgyfq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.316326.xyz/gtjuyzbeki.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtsnryesmt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gtevjdofnf.html

================================================================================
来源：http://hz.wangdashe.top/gtmwhbeagt.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtfnhknmvf.html

================================================================================
来源：http://hz.hywenlv.cn/gthmyjzeso.html

[R01] shebang 与严格模式
来源：http://hz.dianchejie.cn/gtelrtjfsy.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtjcnqdkou.html

set -euo pipefail
来源：http://hz.mhx1999.top/gtszyfjxop.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtrtmosfhp.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gtssgxguyp.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtvroebfaf.html

readonly PI=3.14
来源：http://hz.andypj.xyz/gtbtzvqukf.html

[R04] 位置参数
来源：http://hz.meibo888.top/gtkwfbhqmq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtgpzrcnqe.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gtfgtyvsbo.html

name="${1:-default}"
来源：http://hz.yvedp.cn/gtajkpdwmi.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gteedgnqys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtpbxjnrgx.html

[R07] if 判断文件
来源：http://hz.redwolf501.top/gtppgpnxkd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtrsbxyeau.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtxruyuruw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hongshengwenyu.top/gtvhnchpsq.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtydsyskrd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.0kj1m.cn/gtncdhzmbb.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtvollpeid.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtaiogxrqg.html

[R11] case 多分支
来源：http://hz.9152youxi.cn/gthlryelck.html

case "$1" in
来源：http://hz.jianghu66.top/gtktrguosy.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtulfkymei.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtkydjxeru.html

*)     echo "未知命令" ;;
来源：http://hz.c1oappe.top/gtnbgluabx.html

esac
来源：http://hz.0kj1m.cn/gtzfimrarq.html

[R12] for 遍历文件
来源：http://hz.zhongyouzk.top/gtfgjijoyu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.svipenyu.cn/gtjonjsieq.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtootfuttv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtolikjglc.html

[R14] C 风格 for
来源：http://hz.tanke756.top/gtqjiiboff.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gotoacloud.top/gtxjnnzghe.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gtjarwxerl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtxdxgbmgp.html

[R16] until 等待条件
来源：http://hz.vqdsnc.cn/gtxkybhjzv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtvzphbbkz.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtomcwrbel.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtwoyoubwb.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtfqjxneve.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tianlin.xyz/gtntsihnry.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtxnymqrrn.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtlyxxjyhu.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtmqodvujx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtxyyjwoef.html

[R21] 字符串长度
来源：http://hz.guowangkeji.top/gtwykxumic.html

echo "${#s}"
来源：http://hz.birdmap.top/gtrdawdfxz.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtkcwybizu.html

echo "${s:0:5}"
来源：http://hz.shuidangran.top/gtdiyefzfx.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gthhefgrus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gttnnckrup.html

[R24] 大小写转换
来源：http://hz.chenzaomai.com/gtnwgulcts.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gtlpmlrsup.html

[R25] 去后缀 / 去前缀
来源：http://hz.nwbrower.top/gtbxtjubef.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hywenlv.cn/gtfxqmevwb.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gtpxtiuqbj.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtukymeose.html

[R27] 算术展开
来源：http://hz.sysykeji.top/gtwdjdfmoi.html

echo $((1 + 2 * 3))
来源：http://hz.ppjwa.cn/gtxmrryzlo.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtkyxykelf.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinghuilouyu.cn/gtuimaanxb.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtbuzjezsr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtrlxuzirk.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtgsonblgt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhiwuduotai.top/gteoiphmkc.html

[R31] 局部变量
来源：http://hz.ppjwa.cn/gtqkeajuwi.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtpmsxohuv.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gteihmylje.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cqqwz.cn/gttzzvlwdg.html

[R33] 捕获错误并提示行号
来源：http://hz.xuetiantiany.cn/gtbhehetuy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtwssvsdgk.html

[R34] 退出时清理
来源：http://hz.kuanghao11.cn/gtbxozddrx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtvshrbpnk.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtlmediwui.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zdqjudy.top/gtwicaybys.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtouxahity.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtgtpfofwi.html

[R37] 把输出赋给变量
来源：http://hz.guannengcc.top/gthmohsjvx.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtdwapybhw.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtzckqxjkg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtsghxzqnh.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtffsrpbmx.html

cmd > out.log 2>&1
来源：http://hz.9152youxi.cn/gtoyzipwvk.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtnfblbivn.html

echo "log" >> out.log
来源：http://hz.yangfankeji.com/gtxfoibmcb.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtwifhhspd.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtnnkgxwcj.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtwpxbbxgt.html

wc -l < a.txt
来源：http://hz.ydjk.org.cn/gttbkdvkkc.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtdlkamaqm.html

find . -name "*.log" -type f
来源：http://hz.daria6918.cn/gtyylsvvvc.html

[R44] 按修改时间查找
来源：http://hz.hfpthk.cn/gtpibugdhj.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gtgpyoaice.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gthcbdxuao.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gtxqrkrugw.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtutekaiie.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtxvyarjwe.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtcfkqyxgr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtccplcntx.html

[R48] awk 取指定列
来源：http://hz.yanxiufei.cn/gtmfdqumoq.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtdvwybuhh.html

[R49] awk 带条件
来源：http://hz.jinqigfzy.top/gtvzydczta.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtukqsbffn.html

[R50] awk 求和
来源：http://hz.guowangkeji.top/gtaejqrhey.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nanxinkj.top/gtavttkjbq.html

[R51] 排序去重取前几
来源：http://hz.nanxuanxn.top/gtlhkcluik.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtzgjmcoye.html

[R52] 统计行数
来源：http://hz.hnqzz.top/gthbbanqqn.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtimcfdugi.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtaklvsekv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtbwwsuuwc.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gttyeeyvmd.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gtztuqtuyy.html

[R55] 压缩与解压
来源：http://hz.yj20258.top/gtjdnessdi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtifglboyg.html

[R56] 远程拷贝
来源：http://hz.yj20258.top/gtxpgobdwj.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtvmqatuke.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtljyvmgtw.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtoelczjci.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gtjcbufmsi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ppjwa.cn/gtxyrutxwq.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtxevjxcxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtpnalblgg.html

[R60] 只看 HTTP 状态码
来源：http://hz.andypj.xyz/gtkklwmtik.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtfmgjfywr.html

[R61] 磁盘占用
来源：http://hz.cheryme.top/gtbdnvbbko.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtnkbwsauo.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gtphscaokg.html

du -ah . | sort -rh | head -10
来源：http://hz.yj202588.top/gtnadlefkd.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtzdphiorv.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtidmjqyqk.html

[R64] 结束进程
来源：http://hz.jinyuanbaomall.cn/gtjzizsvmk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtizqbijod.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gtzbeulzfb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtzvdlrxwq.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gteizfsafw.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtjmrvrkag.html

[R67] 生成随机十六进制串
来源：http://hz.hfpthk.cn/gtwikwigsd.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtyqhwouyi.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtnaohzdbb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nwbrower.top/gtoguculaw.html

[R69] 生成随机密码
来源：http://hz.yongpay.top/gtpjpbmudy.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuetiantiany.cn/gtpnhflxjb.html

[R70] 时间戳与互转
来源：http://hz.tianlin.xyz/gtpvxcouvq.html

date +%s;  date -d @1700000000
来源：http://hz.hysaishi.cn/gtwnzcdqtj.html

[R71] 日期格式化
来源：http://hz.zhijiandao.cn/gteeqzmrmu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtawyucxev.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtkgsubsal.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtjrlrxdyk.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gthvsvlpdv.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtudbjbash.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtsohmhanz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtfrdbezea.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtrkecqjqa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangkeji.top/gtxdogjcxx.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtfdngslmj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtqkazzbfc.html

[R77] 读取用户输入
来源：http://hz.zhoulong.xyz/gtqdxyxyph.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gtyulnoaoo.html

[R78] 交互式菜单
来源：http://hz.aibaodan.cn/gtteznofek.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gttwtghlrr.html

[R79] 解析命令行选项
来源：http://hz.pycfn.com/gtcvuqclsf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhijiandao.cn/gtdjwfcpfm.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgfzy.top/gtbdkkpuek.html

time ./run.sh
来源：http://hz.xinyue.icu/gtmboaxkog.html

================================================================================
来源：http://hz.daria6918.cn/gtxcurcqnb.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtakljsjng.html

================================================================================
来源：http://hz.hywenlv.cn/gtqvpqbkiw.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtrxkbnzqw.html

#include <stdio.h>
来源：http://hz.jyoumei.cn/gtencyfacp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuanzx.com/gtlwqoivua.html

[S02] C：变量与格式化输出
来源：http://hz.havefunace.top/gtzlvnkrlp.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigufen.top/gtzjmcygtg.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtvoctdjmp.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtcvkehyhb.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtuflwirnm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtrvswanhf.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtudptynsv.html

strlen(s)
来源：http://hz.cucudq.cn/gtuddtjyxe.html

[S06] C：字符串比较
来源：http://hz.tanke756.top/gtwafhpcsk.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtwuvvmdmz.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gtkwlnnydk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jiagoushi.top/gtwfrxozuj.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtpnoovvez.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtzoxsbdvg.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gteoikfwyo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hongshengwenyu.top/gtpfzflyhx.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtlhoeyaox.html

int *p = &a;  *p = 5;
来源：http://hz.xuetiantiany.cn/gtkglntqxu.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gtxxudoktz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtkgjxwqss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gtdwpidlli.html

fclose(f);
来源：http://hz.gotoacloud.top/gtedguakvk.html

[S12] C：写文件
来源：http://hz.yanxiufei.cn/gtdyxbbjtb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zdqjudy.top/gtfqwynmvl.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtkbcnigcr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtbbfhxdle.html

[S14] C：枚举
来源：http://hz.ywan-chungtsiang.top/gtmapnialt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigufen.top/gtzepyxpev.html

[S15] C：类型转换
来源：http://hz.zdqjudy.top/gtbvmxtpbm.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtdstjdzox.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gtiraejufv.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtkmegwwbx.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gtwldxtayu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtehvaculb.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gttgbzvlzl.html

int main(int argc, char **argv)
来源：http://hz.tianlin.xyz/gtacardbib.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtujufvmyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtwoqyegrj.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtnofhetzb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtpffrethh.html

[S21] C：字符类别判断
来源：http://hz.wangdashe.top/gtsopfytab.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cdnleiting.top/gtjnzlnlat.html

[S22] C：字符串转数字
来源：http://hz.smart0.xyz/gtjodtieri.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtepjzqdkd.html

[S23] C：随机数
来源：http://hz.andypj.xyz/gtatfuonde.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtfcbtgzow.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gthvqleslm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtpmxxitqp.html

[S25] C：内存拷贝
来源：http://hz.xylfe.cn/gtqedplbzm.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtqfrurioj.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtnvcmtvqr.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtphjxizbu.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gtafkgeuut.html

const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtojeyiyrw.html

[S28] C：静态变量
来源：http://hz.xylfe.cn/gtolkwvszp.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtkiwnzulw.html

[S29] C：变参函数
来源：http://hz.316326.xyz/gtqmkdnezi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.meibo888.top/gtnndaxtad.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtdlqivdxn.html

#ifndef X_H
来源：http://hz.nwbrower.top/gtqasqwlfs.html

#define X_H
来源：http://hz.sufxvd.cn/gtiyvliopp.html

#endif
来源：http://hz.mhx1999.top/gtnfccjkgp.html

[S31] C++：Hello World
来源：http://hz.sysykeji.top/gtioxpuryp.html

#include <iostream>
来源：http://hz.yuxming.cn/gttexszmyv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gtoqptigcf.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtqysylwxn.html

std::string s = "hi";  s += "!";
来源：http://hz.haohaochexian.top/gtrmmihrvt.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtztpvbnol.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gthtepteiy.html

[S34] C++：遍历 vector
来源：http://hz.cucudq.cn/gtfegjvvkr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtmirbmmxp.html

[S35] C++：map
来源：http://hz.jinyuanbaomall.cn/gtfzxtmpbt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtmsoousuq.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtxruivmcl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gteqcrpigi.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtmzrrshkz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yonumen.top/gthwvwfqxn.html

[S38] C++：排序
来源：http://hz.jlsjyb.cn/gtbratncta.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtjowcfypm.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtcbizokyh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgufenzy.top/gtbscgutqq.html

[S40] C++：查找元素
来源：http://hz.ehwqpu.com/gtszxtzych.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtmjcjkmje.html

[S41] C++：类与构造函数
来源：http://hz.quarkkingdee.top/gtjuytwjio.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daxiang520.top/gtqbgaablg.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtujporhrz.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gttjpnbcuy.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gtrhlegllu.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtjabrisut.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtrjlobbzn.html

void inc(int &x) { ++x; }
来源：http://hz.dianchejie.cn/gtcftivpxy.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gthocdzwpc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ybcxt.top/gtgqbdkcon.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtlyyunnpb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gthwsujrta.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gtfzlapqgd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuxming.cn/gtqzyupxfh.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtcbnniisu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtdbgppafh.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtynszacoi.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtezlzpdop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtowcgfyat.html

[S50] C++：格式化数字
来源：http://hz.cucudq.cn/gtzgqfvxdz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtacvfmsob.html

[S51] C++：显式类型转换
来源：http://hz.redwolf501.top/gtougckvby.html

static_cast<double>(a) / b
来源：http://hz.9152youxi.cn/gtdyeelpvv.html

[S52] C++：const 与 noexcept
来源：http://hz.nwbrower.top/gtiiclzkzy.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtszqjlwxl.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtxfzuihmu.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtosybxorv.html

[S54] C++：异常处理
来源：http://hz.kuanghao11.cn/gtczsocjdc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtywiqufkk.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gtpvapabuh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtgpftxqih.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtuqbciqts.html


<!-- 参考信息 -->
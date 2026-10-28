代发 wailian999

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtlsyhlqlr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtekcqpxao.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtpuxeerdg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtjdimtokg.html

[Q78] 当前时间
来源：http://hz.jqgfzy.top/gtxjwwprjo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.9152youxi.cn/gtgewtfmkd.html

[Q79] 字符串拼接
来源：http://hz.jinqigfzy.top/gtciywvzlo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzhubu.top/gtelnjdhaz.html

[Q80] 字符串截取
来源：http://hz.daxiang520.top/gtwcrycsvc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtiqlwidjs.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtgmfsetwo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtmotghvqa.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtplwjgyls.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gtslivjyhe.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gttjegkpgs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hfpthk.cn/gtkhnkovga.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtejblcjdc.html

SELECT TRIM(name) FROM users;
来源：http://hz.yonumen.top/gtjpzfirkb.html

[Q85] 数值取整
来源：http://hz.ybcxt.top/gtttjphgax.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtezpjvpnr.html

[Q86] 读取 JSON 字段
来源：http://hz.jinyuanbaomall.cn/gtkskleecs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gttlmvevgm.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtcjvekufd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gthuvzcmmi.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtxqbtxizu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtpyixkezk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtvrwyatvx.html

[Q89] 判断表是否存在
来源：http://hz.jianghu66.top/gtlafaogop.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtkujbirsp.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtnmypbmww.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.redwolf501.top/gtkdfpzfzv.html

================================================================================
来源：http://hz.hysaishi.cn/gtrgjxqeuv.html

R. Bash 专题
来源：http://hz.9152youxi.cn/gtlbfhuknt.html

================================================================================
来源：http://hz.dashuyun.cn/gtsixiilkc.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtybcuzbkb.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtyfaeduba.html

set -euo pipefail
来源：http://hz.yj202588.top/gtexvinihb.html

[R02] 变量赋值与使用
来源：http://hz.zhongyouzk.top/gtrlyaslvl.html

name="Tom"; echo "$name"
来源：http://hz.316326.xyz/gtviqbxjbz.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gtuqfdqioa.html

readonly PI=3.14
来源：http://hz.yuxming.cn/gtkbawflbf.html

[R04] 位置参数
来源：http://hz.gotoacloud.top/gtxfikwbok.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtqrjrdrkm.html

[R05] 参数默认值
来源：http://hz.shzxlz.cn/gtdqkzlauv.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtuchjqlsj.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtddbabkpi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtdlonbwdd.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtthqbfpcw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtheqcngqd.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gtzydusuif.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtpxcirken.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtihsywrry.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhoulong.xyz/gtybhrhefs.html

[R10] 正则匹配
来源：http://hz.yuxming.cn/gtihtcyula.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtknjmbkmx.html

[R11] case 多分支
来源：http://hz.cdnleiting.top/gtxzzhayvy.html

case "$1" in
来源：http://hz.jinqigfzy.top/gtkxhgrref.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangtech.top/gtiqahdteo.html

stop)  echo "停止" ;;
来源：http://hz.snrcjt.cn/gttpzqzota.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtrhhhignj.html

esac
来源：http://hz.yangfankeji.com/gttebiqfor.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtbqqzuhgb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gthevxvmvn.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtdopudiou.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yongpay.top/gtspbvkwqs.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtkskxkjnf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtkgzgttjq.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtgbpftqma.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gttmcvyvpt.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gteslsavuf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtifbkunuq.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtfhrgzcze.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtcbzcdtbx.html

[R18] 遍历数组
来源：http://hz.chenjidiqi.icu/gtayuaudlz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtcfbtfpxj.html

[R19] 数组长度
来源：http://hz.sufxvd.cn/gtrnapajtz.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtablaxtlc.html

[R20] 关联数组（字典）
来源：http://hz.meibo888.top/gttqipkixp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtfbutvvav.html

[R21] 字符串长度
来源：http://hz.wangdashe.top/gtqujslcoo.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtbpylikwz.html

[R22] 截取子串
来源：http://hz.bjfxy.top/gtcnrwtbmb.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtetlrnaku.html

[R23] 字符串替换
来源：http://hz.fzhhl.top/gtspalbtlh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gtgphliqaq.html

[R24] 大小写转换
来源：http://hz.quarkkingdee.top/gtagnldvno.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtngahsofi.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gtcxqyidwx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gtkjgvibgs.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtgupluvxd.html

now=$(date +%F); echo "$now"
来源：http://hz.sxryk.cn/gtinrngwmg.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtzndcprte.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtktdphokt.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtqpjkdtng.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigfzy.top/gtoxtwpcda.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtbedzgsdb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gteudiqcfd.html

[R30] 函数返回状态码
来源：http://hz.zhaomingkeji.xyz/gttqwvjbpp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydjk.org.cn/gtnwoetdwx.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtkjxofbtg.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtckpzmirc.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangtech.top/gtdhsdxbzz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydzc1.top/gtrikywkzi.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgfzy.top/gtauycckqj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gttmvjqpxr.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gtrhrgsgpp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtllbmmlzs.html

[R35] 后台执行并等待
来源：http://hz.0kj1m.cn/gtxjabkrut.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tianlin.xyz/gtjzdcfvmz.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gtmgdmxorv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gtdudbwfzz.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtqmvcojpc.html

files=$(ls -1)
来源：http://hz.xziqi.cn/gtqnstbcin.html

[R38] 管道串联
来源：http://hz.jlsjyb.cn/gtgrhudnot.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cheryme.top/gtdgocyabf.html

[R39] 重定向标准输出与错误
来源：http://hz.snrcjt.cn/gtioarybsh.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtjraizxit.html

[R40] 追加写日志
来源：http://hz.zhixingplan.top/gtihdftyng.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtdpfryrys.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtzgekiumm.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gthilwhqwj.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtqjevhkou.html

wc -l < a.txt
来源：http://hz.guannengcc.top/gtpwuazxww.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtdxuxnajg.html

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gttzauupbp.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gtoimhexwq.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtzpcexwlf.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtxwornctu.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtrmafdbjg.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtjykjddoz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jiagoushi.top/gtbrouzmdl.html

[R47] sed 单行替换
来源：http://hz.nwbrower.top/gtfsiargml.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtjdhyvzug.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtmsxzofqd.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtydewlbbo.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtgraqwcbq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtvomtzpsc.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtwpkatlpo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtyztwbkan.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtbtizgphu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinqigufen.top/gtmjqyyfcm.html

[R52] 统计行数
来源：http://hz.aizwys.cn/gtnmiwbino.html

wc -l a.txt
来源：http://hz.hammf.cn/gtfgzluqgg.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gttsgcbmfa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtgqfsytjf.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtlwzttaht.html

diff a.txt b.txt
来源：http://hz.xuetiantiany.cn/gtwgjhgeny.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtufbzplts.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtqsojakmv.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtebuvugmh.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gttajptehm.html

[R57] 远程执行命令
来源：http://hz.kuanghao11.cn/gtzipgkaeo.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gttsvpglyx.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtznxhepyy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtkbyqdvmc.html

[R59] 发 POST JSON
来源：http://hz.nwbrower.top/gtdllgxzyp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtcugpbjyd.html

[R60] 只看 HTTP 状态码
来源：http://hz.bjfxy.top/gtipyouhwh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hywenlv.cn/gtptdnjxfg.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtbnggjvoh.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtyswjgpgb.html

[R62] 找最占空间的文件
来源：http://hz.zhijiandao.cn/gtrjlwnceu.html

du -ah . | sort -rh | head -10
来源：http://hz.fengsongda.top/gtqmcbkhtf.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtqvekbprq.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtskikxbil.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtrcrqgtvm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guannengcc.top/gtzblfjgjg.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtbsmvftzf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtrdberrpc.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtrzuxrymy.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtsefdxqoo.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtmhzxiwnz.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtylhkscqw.html

[R68] 计算文件校验值
来源：http://hz.ywan-chungtsiang.top/gtmndbmthm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtyrfilcjo.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtmqrstalg.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtgirwjysp.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtwlpzvidy.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtauxqakqd.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtvbpwjorw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtsnvwcfbx.html

[R72] 等待端口就绪
来源：http://hz.zhoulong.xyz/gtpxiircvw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtwschleho.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtnlvhcktm.html

split -l 1000 big.log part_
来源：http://hz.guannengcc.top/gtwycpjhhg.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gtjzxcyehg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gtiqmiguup.html

[R75] 导出环境变量
来源：http://hz.yueranfly.top/gtctwsmcbj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtciclqvil.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtzefaojjw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtrabkwfug.html

[R77] 读取用户输入
来源：http://hz.cashguo.top/gtluxuyyqw.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtatumibhk.html

[R78] 交互式菜单
来源：http://hz.yuxming.cn/gtebglrryy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sufxvd.cn/gtnunqhenp.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtzwsaorsy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtmkvsnvug.html

[R80] 查看脚本执行耗时
来源：http://hz.xingfuxueyuan.xyz/gtgiqzrnfy.html

time ./run.sh
来源：http://hz.xziqi.cn/gtnmniwtvw.html

================================================================================
来源：http://hz.guowangkeji.top/gtgnjtivbu.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gtlrxhokqu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtcuqjnqwg.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtdzlqcgau.html

#include <stdio.h>
来源：http://hz.quarkkingdee.top/gtcigphntn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtcnznqiam.html

[S02] C：变量与格式化输出
来源：http://hz.nwbrower.top/gtnjlabgoh.html

int a = 10; printf("%d\n", a);
来源：http://hz.svipenyu.cn/gtbmlfefpp.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtpjnbnwds.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtpxvkelen.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtoznljyyn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.mhx1999.top/gtjxvsmaes.html

[S05] C：字符串长度
来源：http://hz.cdnleiting.top/gtjoxxlalo.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtkzefzxdx.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gtnkrigrma.html

strcmp(a, b) == 0
来源：http://hz.havefunace.top/gtrhofwals.html

[S07] C：数组遍历求和
来源：http://hz.ydzc1.top/gtkwlltuna.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtcojzihdw.html

[S08] C：动态内存分配与释放
来源：http://hz.ydjk.org.cn/gtpksajmcu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtxrnkceuq.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtdtxxbtfh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.316326.xyz/gtfqtwzble.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtzfaqnmey.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtxowveret.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtljixpxmn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gttstmmdmx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtqmdzpmys.html

fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtnmpnutnr.html

[S12] C：写文件
来源：http://hz.zhengqikj.top/gtcvwmccmk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtlbztmayu.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtzyubkvtl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtmlblkgax.html

[S14] C：枚举
来源：http://hz.ehwqpu.com/gtusfejsrs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtqmvynxyb.html

[S15] C：类型转换
来源：http://hz.sysykeji.top/gtcdafrxdv.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtkzvoktlm.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gttvzsjvei.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtcepgmfsa.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtizbmzpoh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtggxrwmwa.html

[S18] C：命令行参数
来源：http://hz.xinyue.icu/gtsacwadde.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gtcifhuquq.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gtyjouctpb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtabfmvyao.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtybiuiepx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtvrfmfjvw.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtfrzvupib.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zycfv.cn/gtyretblxg.html

[S22] C：字符串转数字
来源：http://hz.jlsjyb.cn/gtwtepekcc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xylfe.cn/gtixggkfyk.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtdciofljp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shuidangran.top/gtzeefszjy.html

[S24] C：获取本地时间
来源：http://hz.nwbrower.top/gtvwjbzkdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtewuvqrjj.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtrwqnghpy.html

memcpy(dst, src, n);
来源：http://hz.nanxuanxn.top/gtosmuykpc.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtyendlxkp.html

memset(a, 0, sizeof a);
来源：http://hz.xylfe.cn/gtmozitruy.html

[S27] C：定义常量
来源：http://hz.zhixingplan.top/gtojljvwcs.html

const double PI = 3.14159;
来源：http://hz.sysykeji.top/gtdelztkum.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gtiaybebwy.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtuhtnijtu.html

[S29] C：变参函数
来源：http://hz.zdqjudy.top/gtdwsnmlxo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuxming.cn/gtdvnpezcy.html

[S30] C：头文件保护
来源：http://hz.ehwqpu.com/gtuaoqsbps.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtogwnwger.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtjnncuxhm.html

#endif
来源：http://hz.shangyingyoupin.top/gtputuojuf.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtizavkvlq.html

#include <iostream>
来源：http://hz.havefunace.top/gtordbnopc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinghuilouyu.cn/gttjespwod.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gtbuzqvlmq.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtggvjezux.html

[S33] C++：vector 增删
来源：http://hz.hnxiangtu.top/gtcbrfbyvg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigufen.top/gtahmeqepc.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gttydmnuch.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gttxngbtyr.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtqhvlakgh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtwtixovtk.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtdbrmjpfm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gttooejhkj.html

[S37] C++：set
来源：http://hz.sxryk.cn/gttvmthlmn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtpgxjkvbq.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtguzdbxee.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtwocpmhpb.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgfzy.top/gtathphkav.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gtvwedjftm.html

[S40] C++：查找元素
来源：http://hz.havefunace.top/gtxjyaxosx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtccafnihx.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtyawswztm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ehwqpu.com/gtytnttpqw.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtyfkymqjk.html

class B : public Base { public: void f() override {} };
来源：http://hz.pengpengdd.cyou/gtwagprbww.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtsgihzniq.html

auto p = std::make_unique<int>(5);
来源：http://hz.haohaochexian.top/gtkaqarsvp.html

[S44] C++：引用传参
来源：http://hz.yonumen.top/gtraowpypf.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtklcevnkm.html

[S45] C++：lambda
来源：http://hz.tanke756.top/gtsnbzhaeq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gtddmwlskt.html

[S46] C++：函数模板
来源：http://hz.cheryme.top/gtddrwjdue.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xziqi.cn/gtcczpidhl.html


<!-- 参考信息 -->
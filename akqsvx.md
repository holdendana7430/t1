代发 wailian999

[Q80] 字符串截取
来源：http://hz.aizwys.cn/gtmgertsdg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daria6918.cn/gtddprwxvo.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtxifljjvp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtyugmrity.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtuddxhirj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jyoumei.cn/gtiyyzajob.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtlueswvlv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtwuerotvb.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtcbicjitb.html

SELECT TRIM(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtjsilarxj.html

[Q85] 数值取整
来源：http://hz.chenjidiqi.icu/gtlwnpyuaa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtovqzvzqt.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gtyzdvrhag.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtaqumxxas.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtcifwovbw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtatnzxygr.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtmzpszjkf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtvcckbodx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtyvvetrql.html

[Q89] 判断表是否存在
来源：http://hz.9152youxi.cn/gtyootwrbv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gthlnmwvor.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtsfuxhcje.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxuanxn.top/gttleqdvof.html

================================================================================
来源：http://hz.fengsongda.top/gtsroytxck.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtjrulteiz.html

================================================================================
来源：http://hz.fzhhl.top/gtlbwupzzb.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtfbissjss.html

#!/usr/bin/env bash
来源：http://hz.iojbl.cn/gtikbtwnzw.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gtjziyqtrm.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtyjfnliqn.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtexywhnxx.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtlgotiyhf.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtxdnhizrt.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtifreoqqc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dashuyun.cn/gtonxryjfw.html

[R05] 参数默认值
来源：http://hz.yueranfly.top/gtuivstwuv.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtxuabpreh.html

[R06] 判断命令是否存在
来源：http://hz.jinghuilouyu.cn/gtwkatznya.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gttbnkkvqi.html

[R07] if 判断文件
来源：http://hz.dianchejie.cn/gtefozyuuc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhongyouzk.top/gthgqsakfb.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gtxuietxfx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtbzppmeuc.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gtrdnazcmk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daxiang520.top/gtpsiecgdz.html

[R10] 正则匹配
来源：http://hz.nanxuanxn.top/gtmlhdqnut.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtesnnetzy.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtbjvbzqec.html

case "$1" in
来源：http://hz.redwolf501.top/gthigwcjqz.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gthpzzpfvk.html

stop)  echo "停止" ;;
来源：http://hz.sxryk.cn/gtkblwirju.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtqxxiqmnv.html

esac
来源：http://hz.yvedp.cn/gthgfkocdq.html

[R12] for 遍历文件
来源：http://hz.xingfuxueyuan.xyz/gtqzyjwpzz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtbpsldjpg.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtmvwrnapo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtkljqrreq.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gthpevuczy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gtlewjybtg.html

[R15] while 逐行读文件
来源：http://hz.shuidangran.top/gtwjvkcdym.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtmytebskp.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtfxmgvlii.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gtkrltnryn.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtwhmloaaz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtdqbkgtvz.html

[R18] 遍历数组
来源：http://hz.ywan-chungtsiang.top/gtfxzpidcp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtqebipmht.html

[R19] 数组长度
来源：http://hz.shangyingyoupin.top/gtmllxkgie.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtnrtwkxak.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtyhvoyetr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtofklqrea.html

[R21] 字符串长度
来源：http://hz.vqdsnc.cn/gthgomtldr.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtssqrnppx.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtdciruyiy.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtbgksgnnl.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtexxhdwgr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shuidangran.top/gtoszsnbdl.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtqnwruisi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gttaxexpko.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtbhldfshi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tanke756.top/gtnlaopaua.html

[R26] 命令替换
来源：http://hz.kuanghao11.cn/gtcqdejenk.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gttwpotkff.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtryqdhzug.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gtfbtzpnqd.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtqvuythap.html

echo "scale=2; 10/3" | bc
来源：http://hz.quarkkingdee.top/gtvbjmisez.html

[R29] 定义函数
来源：http://hz.jlsjyb.cn/gtjxpwdqjq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtfdzetiak.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gtshfgfpwc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.52xcode.cn/gtcsyqlmjs.html

[R31] 局部变量
来源：http://hz.shanyushiyangtech.top/gtjhydvsbx.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtljbjviav.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gtfgdcdizp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtilurkrzi.html

[R33] 捕获错误并提示行号
来源：http://hz.shzxlz.cn/gtgwkqvlrp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.vqdsnc.cn/gtiozdavwx.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gtcjkdsxzx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtdrdknszx.html

[R35] 后台执行并等待
来源：http://hz.guowangkeji.top/gtsilvkehd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtiabajsso.html

[R36] 并发执行多个任务
来源：http://hz.sxryk.cn/gtacqlcokq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtdhypxdem.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtcxizphzr.html

files=$(ls -1)
来源：http://hz.ehwqpu.com/gteseiiiaf.html

[R38] 管道串联
来源：http://hz.gogol.net.cn/gtpfebceli.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtwfsgdhzp.html

[R39] 重定向标准输出与错误
来源：http://hz.cucudq.cn/gtbmxgkawf.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gtvqafdxdw.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtmefmksef.html

echo "log" >> out.log
来源：http://hz.ppjwa.cn/gtzttwqgxw.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtxtslqxcs.html

cmd >/dev/null 2>&1
来源：http://hz.aibaodan.cn/gtfgxlpvhx.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtqicbqalh.html

wc -l < a.txt
来源：http://hz.jinqigufen.top/gtwetejnqv.html

[R43] 按名字查找文件
来源：http://hz.hnqzz.top/gtaurrrfml.html

find . -name "*.log" -type f
来源：http://hz.svipenyu.cn/gtoasjmgdd.html

[R44] 按修改时间查找
来源：http://hz.zycfv.cn/gtjruggrmo.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtwbbofhxs.html

[R45] 批量删除
来源：http://hz.yj20258888.top/gtupchhzwr.html

find . -name "*.tmp" -delete
来源：http://hz.yueranfly.top/gtpoxgexyo.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtfhbrdcro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtspcgonqf.html

[R47] sed 单行替换
来源：http://hz.hammf.cn/gtdqkpcjvw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtacmstvfc.html

[R48] awk 取指定列
来源：http://hz.yj202588.top/gtdxgmvsys.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gteqlkbhdz.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtfxrguvvw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtuvpwegsl.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtazlaxkfn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtuxyuwsxx.html

[R51] 排序去重取前几
来源：http://hz.daxiang520.top/gtshdjndsf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtcigmfnqa.html

[R52] 统计行数
来源：http://hz.nanxinkj.top/gthfhzisyt.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtcphzzqxr.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gtvthnirmc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtcwlrznse.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtupgbbgsg.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtgszcgkiw.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtkhrqtxnt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtajflkmbp.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtnlvcqwmm.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtmfysckqs.html

[R57] 远程执行命令
来源：http://hz.pengpengdd.cyou/gtgyqelkns.html

ssh user@host 'uptime'
来源：http://hz.cheryme.top/gtixxubmmf.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtllwoetcx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gthxmcynzn.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtqzldwfwt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtzjzxroeq.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtvappfwdp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtyhowlegl.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gtsnxrycik.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtftartrzs.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtkydtoecy.html

du -ah . | sort -rh | head -10
来源：http://hz.mhx1999.top/gtzoulqthw.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtjglolhim.html

free -h;  ps aux | grep nginx
来源：http://hz.guannengcc.top/gtlopnzayd.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtjempmfsl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gtsssvxnhn.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtloeyfzke.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xuetiantiany.cn/gtfhafadzn.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtdbvgtwoe.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangtech.top/gtauhlqdrz.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtkbsiniqa.html

openssl rand -hex 16
来源：http://hz.jqgfzy.top/gtzqzvlquh.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gthgbkbaoo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtgymmzfau.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtecpjxiwz.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gthmikkebb.html

[R70] 时间戳与互转
来源：http://hz.yj20258888.top/gtnxnanwmh.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gtgewlpoqg.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtfopzions.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hammf.cn/gtqovcezwi.html

[R72] 等待端口就绪
来源：http://hz.meibo888.top/gtpyezknms.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtdjmtuzbm.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gttnzefkvf.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtyvpcvifu.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtvdxvmnkt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtvpbyrfiu.html

[R75] 导出环境变量
来源：http://hz.yonumen.top/gttplznlmj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtkyrjeghr.html

[R76] 使用临时文件
来源：http://hz.ydzc1.top/gtfinbyluv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtjzpohqye.html

[R77] 读取用户输入
来源：http://hz.yj20258.top/gtodnjksvq.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtjhcmxtro.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtjjcofowz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtejujjpax.html

[R79] 解析命令行选项
来源：http://hz.pycfn.com/gtmltyjbbw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gttdyrlawx.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtcvdzzhlm.html

time ./run.sh
来源：http://hz.smart0.xyz/gtymznuice.html

================================================================================
来源：http://hz.sweek.top/gtpvxcnkkq.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtrnaspzbq.html

================================================================================
来源：http://hz.jyoumei.cn/gtrpdqmdol.html

[S01] C：Hello World
来源：http://hz.birdmap.top/gtqxtgrfzy.html

#include <stdio.h>
来源：http://hz.chenlongwang.top/gtrqqqbtag.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtnrkqyoxp.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258888.top/gtswggjnhp.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigfzy.top/gtlcsnoltq.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gtwhxezkwz.html

int x; scanf("%d", &x);
来源：http://hz.jinyuanbaomall.cn/gtsatzegzl.html

[S04] C：字符串复制
来源：http://hz.yangfankeji.com/gtsqdfqols.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtqhhirdzr.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gttaytwzcv.html

strlen(s)
来源：http://hz.zhijiandao.cn/gtzpowuazy.html

[S06] C：字符串比较
来源：http://hz.hnxiangtu.top/gtngnovfgr.html

strcmp(a, b) == 0
来源：http://hz.nanxuanxn.top/gtvoqcxikm.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtllvqqryp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtskkbwkkk.html

[S08] C：动态内存分配与释放
来源：http://hz.jianghu66.top/gtxrnimxxr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gtcecilzbt.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtcmxzyjju.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtapulxwsb.html

[S10] C：指针与解引用
来源：http://hz.yangfankeji.com/gttutknqnb.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtrwywxsoz.html

[S11] C：逐行读文件
来源：http://hz.hfpthk.cn/gtdjqmlsao.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cucudq.cn/gttikdyold.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtbpcefaco.html

fclose(f);
来源：http://hz.hongshengwenyu.top/gtywgczbfq.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtzcidjzaj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gthplnatik.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtajbqvltg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtgsfkgevg.html

[S14] C：枚举
来源：http://hz.zhaomingkeji.xyz/gtnosmdvic.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hfpthk.cn/gtghhyzjce.html

[S15] C：类型转换
来源：http://hz.jqgfzy.top/gtjqzvkmyt.html

(double) a / b
来源：http://hz.ivvv.top/gtpbrazfsp.html

[S16] C：位操作置位
来源：http://hz.ivvv.top/gtfscphxrp.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtegivgerz.html

[S17] C：安全拼接字符串
来源：http://hz.xuetiantiany.cn/gtdsdfejao.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtuzcwefdw.html

[S18] C：命令行参数
来源：http://hz.ydzc1.top/gtmdnfahdq.html

int main(int argc, char **argv)
来源：http://hz.ydzc1.top/gtiliolhqf.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtkdfexppe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtytncdhym.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtncrwronl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtuvlnlbok.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtqgkwzxve.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gtywvagpkf.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtnvukuqly.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtqffanjyq.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtnnmaoqgh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtxdxpwlbs.html

[S24] C：获取本地时间
来源：http://hz.c1oappe.top/gtkdhmfsmn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangkeji.top/gtvbumujxs.html

[S25] C：内存拷贝
来源：http://hz.yuanzhike.top/gthcsavlzl.html

memcpy(dst, src, n);
来源：http://hz.hammf.cn/gtzglxnbuq.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtqrjjvxmy.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gtlfzehsvh.html

[S27] C：定义常量
来源：http://hz.vqdsnc.cn/gtuoduhsul.html

const double PI = 3.14159;
来源：http://hz.cheryme.top/gtqfgfkzgo.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gtlweititr.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gttjhmzrme.html

[S29] C：变参函数
来源：http://hz.cqqwz.cn/gtvkqdruht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtwpqjiwjx.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtktowigdi.html

#ifndef X_H
来源：http://hz.aizwys.cn/gtanxbmiai.html

#define X_H
来源：http://hz.havefunace.top/gtpghnkygy.html

#endif
来源：http://hz.shuidangran.top/gtzauzjaee.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtustwdvsc.html

#include <iostream>
来源：http://hz.havefunace.top/gthmoaxnes.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtetgcjojo.html

[S32] C++：字符串
来源：http://hz.pycfn.com/gtscyveevg.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtpadhbuxh.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtzntutzsw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtwjonqtau.html

[S34] C++：遍历 vector
来源：http://hz.zhaomingkeji.xyz/gtayeacgkt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtvirplzxv.html

[S35] C++：map
来源：http://hz.sysykeji.top/gthfbbaqwr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtxwdcosep.html

[S36] C++：unordered_map
来源：http://hz.bjfxy.top/gtfauqaxxj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtnviwkpef.html

[S37] C++：set
来源：http://hz.zhixingplan.top/gtmuyzheci.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtaypreijp.html

[S38] C++：排序
来源：http://hz.tian-w.cn/gtpskqqmyv.html

std::sort(v.begin(), v.end());
来源：http://hz.xylfe.cn/gtbmgnqidi.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtkvfhhegp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtyqrpkrke.html

[S40] C++：查找元素
来源：http://hz.chenzaomai.com/gtkhzoxwlj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtswifnwph.html

[S41] C++：类与构造函数
来源：http://hz.andypj.xyz/gtfrzbtulr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.birdmap.top/gtwtdvtrhh.html

[S42] C++：继承与虚函数
来源：http://hz.yvedp.cn/gtmdseurse.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtzfbqpwcj.html

[S43] C++：智能指针
来源：http://hz.shzxlz.cn/gtkxsawntj.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtnfyxlefo.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtkupumwoq.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtslrxxutz.html

[S45] C++：lambda
来源：http://hz.jqgufenzy.top/gtwbbafhez.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.mhx1999.top/gtygswuhff.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtisvinjhn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtaxeyzpnm.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtcsuhzbcs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.redwolf501.top/gtnnozgppy.html

[S48] C++：逐行读文件
来源：http://hz.yj20258888.top/gtgkcxpppc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtarmrrrya.html

while (std::getline(in, line)) { }
来源：http://hz.tian-w.cn/gtbfgoofue.html

[S49] C++：写文件
来源：http://hz.jianghu66.top/gtoceiscww.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtobfduint.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtlfctmlxb.html


<!-- 参考信息 -->
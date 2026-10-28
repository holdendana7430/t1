代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtlmbwjdna.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtzvdvvbvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtezzknmux.html

[Q74] 强制使用索引
来源：http://hz.meibo888.top/gtvoidfibu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cqqwz.cn/gtlqfkzxmx.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtkheddatv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gteenyhbpy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gthhmkwkol.html

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gtuazfckvj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.smart0.xyz/gtiocdglmu.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gtxjtklqvb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgufenzy.top/gtuhbtnvdc.html

[Q78] 当前时间
来源：http://hz.dashuyun.cn/gtfyjeylhy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhongyouzk.top/gtexrcrcma.html

[Q79] 字符串拼接
来源：http://hz.shangyingyoupin.top/gtdnkxxppd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangtech.top/gtkubhqwoh.html

[Q80] 字符串截取
来源：http://hz.zhixingplan.top/gtkjcgfmgm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guowangkeji.top/gtscspfejp.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtkdarrdkb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ivvv.top/gtyctaihaq.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gtvypputqw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtebrwrzhm.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gttqtlhdji.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fengsongda.top/gtogdtstur.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtgmppjior.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtnmjayvil.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtardntpbe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtrttpmkfx.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtspjdljvz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtxfdsofma.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtikfqbbav.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gttnncubgd.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhiwuduotai.top/gtuqrutqcg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtqsvifggk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnxiangtu.top/gtzluhizer.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtumtbtgbf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtsomrdktx.html

[Q90] 生成序号列
来源：http://hz.sweek.top/gtenlztark.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhengqikj.top/gtgnyikryf.html

================================================================================
来源：http://hz.smart0.xyz/gtmvaqxkdc.html

R. Bash 专题
来源：http://hz.yuxming.cn/gthhoxvgsg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtjzjibdpd.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gtmqegcftl.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtzazxbfbu.html

set -euo pipefail
来源：http://hz.ivvv.top/gtrscnpksy.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtcsmkvkcd.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtbwwgzxcv.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtikltlodb.html

readonly PI=3.14
来源：http://hz.ydjk.org.cn/gtvhjvckda.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gthcbywlrh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtyaqbvsbq.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtvnoypiid.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtidlpabfg.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtoziakngd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.c1oappe.top/gtctqgkrxf.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtpanqtvdf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtoqkgbtdh.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtgfznwpef.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtqtfdgddw.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtnlugmonz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gtjjlthtya.html

[R10] 正则匹配
来源：http://hz.gaohongyu789.top/gtsuwacwcq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gttvwgqjgj.html

[R11] case 多分支
来源：http://hz.gogol.net.cn/gtyhthccaa.html

case "$1" in
来源：http://hz.hysaishi.cn/gtdzqqvxxw.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtmogyiayz.html

stop)  echo "停止" ;;
来源：http://hz.kuanghao11.cn/gtxncskwdm.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtxcleqead.html

esac
来源：http://hz.yj202588.top/gtsmezocoo.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtdwoylwzp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tian-w.cn/gtujlfjwgh.html

[R13] for 计数循环
来源：http://hz.jqgufenzy.top/gtdotqfpgh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtmidpsjkj.html

[R14] C 风格 for
来源：http://hz.sxryk.cn/gtnymbcqpl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtgjwrfdie.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gtqcfsmogp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gtluxbuvzi.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtdepnbuqm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtyozhsyoa.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtmsvbqwkg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jianghu66.top/gtloqofqxv.html

[R18] 遍历数组
来源：http://hz.nanxuanxn.top/gtrkrrkbmu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtoliequku.html

[R19] 数组长度
来源：http://hz.yongpay.top/gtcdqobslx.html

echo "${#arr[@]}"
来源：http://hz.c1oappe.top/gthykizczq.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gtuuruzvqu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtfrvuvhmk.html

[R21] 字符串长度
来源：http://hz.pycfn.com/gtcijjsfmb.html

echo "${#s}"
来源：http://hz.guowangkeji.top/gtunihjpvi.html

[R22] 截取子串
来源：http://hz.smart0.xyz/gtytaubxrn.html

echo "${s:0:5}"
来源：http://hz.yangfankeji.com/gtfgaqpgyr.html

[R23] 字符串替换
来源：http://hz.yuxming.cn/gtouwzotme.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtxyphyxrc.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtouooxxnn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtvkhmzpzc.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtzfbllpcn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.quarkkingdee.top/gtksqtytoj.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gteclrpdqa.html

now=$(date +%F); echo "$now"
来源：http://hz.feifeiyinyue.top/gtddyhpjjd.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtmrifwbbe.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtdlrternf.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtwlujxpbw.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gtumfdyryz.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtbfobdmig.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtsamiykwl.html

[R30] 函数返回状态码
来源：http://hz.yvedp.cn/gtvffkkghw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtajgqsdvn.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtsxammqjv.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtiatuxxfq.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtvqklikyt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gtajhoafzl.html

[R33] 捕获错误并提示行号
来源：http://hz.yanxiufei.cn/gtedggjyqv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtqcvwycqw.html

[R34] 退出时清理
来源：http://hz.jinyuanbaomall.cn/gtaqwecdhi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtclhnixrv.html

[R35] 后台执行并等待
来源：http://hz.c1oappe.top/gtaqxuoihl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtrvxfqkxp.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtxfelhmve.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gtrhefmxyu.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gtlslicnys.html

files=$(ls -1)
来源：http://hz.dianchejie.cn/gtrddlgzpl.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gterljpidd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtmusauvxr.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gtzoqyzraq.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtjewojwfo.html

[R40] 追加写日志
来源：http://hz.cucudq.cn/gtmwajafhd.html

echo "log" >> out.log
来源：http://hz.jiagoushi.top/gtaeodzoua.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtnfrcikkc.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtmdxwffnf.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtprbthjtl.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtjvplamhc.html

[R43] 按名字查找文件
来源：http://hz.bjfxy.top/gtcvkinaye.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gtqwruuqam.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtlsdrihmz.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtcptzuada.html

[R45] 批量删除
来源：http://hz.zhongyouzk.top/gtoswbbspi.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtoypsjfuo.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtapraqtpr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtchmppwra.html

[R47] sed 单行替换
来源：http://hz.daxiang520.top/gtwbhczeeh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtrizgegxr.html

[R48] awk 取指定列
来源：http://hz.cdnleiting.top/gtbvxjzrto.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gteubmjitk.html

[R49] awk 带条件
来源：http://hz.nanxuanxn.top/gtyqqwrkwy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtvtllqlwo.html

[R50] awk 求和
来源：http://hz.yueranfly.top/gtstpvkcyc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtknsxfuum.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gtdjjagtfs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jyoumei.cn/gtxekvibft.html

[R52] 统计行数
来源：http://hz.yj20258888.top/gtypnpuuyj.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtdvmeshhx.html

[R53] 查看文件头与实时尾
来源：http://hz.yueranfly.top/gtxahltnpu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.kuanghao11.cn/gtivgtixsr.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtrsgrunhx.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gtnquzeulq.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtteoqhsvx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gtpxeymzvr.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gtwvqgnliw.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gttwyzkeat.html

[R57] 远程执行命令
来源：http://hz.hnqzz.top/gtsbtpmyrw.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtyesqfgnw.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtpkkfuzzd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtdxmmxjcz.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gtworcbdhg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtrwhpkwmz.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtdabzftmw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hongshengwenyu.top/gtuckbdmpn.html

[R61] 磁盘占用
来源：http://hz.ybcxt.top/gtsjwmikgi.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gtdwhluzmq.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gthmgtelht.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtahorcndq.html

[R63] 内存与进程
来源：http://hz.birdmap.top/gtgzewfanj.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gttgjsqgrz.html

[R64] 结束进程
来源：http://hz.hywenlv.cn/gtdwaasnsz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cheryme.top/gtbnriwget.html

[R65] 查看端口占用
来源：http://hz.pengpengdd.cyou/gthsnepfaf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtxmgdzozh.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtobpfmmqf.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtljkbvssa.html

[R67] 生成随机十六进制串
来源：http://hz.yueranfly.top/gtqxmrzrwq.html

openssl rand -hex 16
来源：http://hz.guowangkeji.top/gtxlfatlrs.html

[R68] 计算文件校验值
来源：http://hz.hongshengwenyu.top/gtgfumrvwq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtzfmhxsoz.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gtellxpvdr.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtjvrotxrn.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtzdlaxroh.html

date +%s;  date -d @1700000000
来源：http://hz.xinyue.icu/gtvqhoeshp.html

[R71] 日期格式化
来源：http://hz.xziqi.cn/gtuvgxpnzs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gttmsamugr.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtheplcfmd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtticvtexq.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gttyyytlxr.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtkbkqghbx.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtxbznnkye.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtknidlhjh.html

[R75] 导出环境变量
来源：http://hz.pycfn.com/gthkhhvupa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtbuwtvtxl.html

[R76] 使用临时文件
来源：http://hz.tanke756.top/gtnutajhkj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtlbrmkkyh.html

[R77] 读取用户输入
来源：http://hz.nanxinkj.top/gtpmfvjrbv.html

read -rp "请输入: " ans
来源：http://hz.ydzc1.top/gtgitnktas.html

[R78] 交互式菜单
来源：http://hz.zhaomingkeji.xyz/gtmbteokec.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.9152youxi.cn/gtniqfcubi.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtukptybyk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.havefunace.top/gtjnabijgy.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtkrxfhtcf.html

time ./run.sh
来源：http://hz.bjfxy.top/gtdmisswgj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtszjpgikj.html

S. C / C++ 专题
来源：http://hz.zhaomingkeji.xyz/gtxpojokur.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthnrfkvfg.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtfhbuhutf.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtjjuyaofu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258.top/gtyggtqblt.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gtiwjydngo.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtdfaztlej.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtqhtkdxle.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtqusvxlhx.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gthsjftvsz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtajzoxcqw.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gtkdtxkalx.html

strlen(s)
来源：http://hz.yj20258888.top/gttpimfbro.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gttfiakxxe.html

strcmp(a, b) == 0
来源：http://hz.yangfankeji.com/gtmqujlksb.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtjfbdkzug.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gthhaajeic.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtdmwwhhdd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dashuyun.cn/gtznmwjisv.html

[S09] C：结构体定义与初始化
来源：http://hz.hongshengwenyu.top/gtqqewqjyl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtctbhnbps.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtkjekvdtf.html

int *p = &a;  *p = 5;
来源：http://hz.gzhubu.top/gtonhovdpp.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtofiayhqc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hongshengwenyu.top/gtdhuraitm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtjjksjeob.html

fclose(f);
来源：http://hz.daxiang520.top/gtnctotmvw.html

[S12] C：写文件
来源：http://hz.xingfuxueyuan.xyz/gtuvfgbnvo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shangyingyoupin.top/gtukpbaoff.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtaireooyc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtobzksufa.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtskituckk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtipvowgmq.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtrnhnyzxb.html

(double) a / b
来源：http://hz.yj202588.top/gtuhoottth.html

[S16] C：位操作置位
来源：http://hz.gotoacloud.top/gtecwyjlbb.html

x |= (1 << 3);
来源：http://hz.aizwys.cn/gttytdkfjm.html

[S17] C：安全拼接字符串
来源：http://hz.chenjidiqi.icu/gtnqwyrkei.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gtemxdzjhj.html

[S18] C：命令行参数
来源：http://hz.haohaochexian.top/gtqvvqoseo.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangtech.top/gtcglyjrro.html

[S19] C：快速排序
来源：http://hz.0kj1m.cn/gtkbwocjpt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gteiitjbbe.html

[S20] C：二分查找
来源：http://hz.redwolf501.top/gtihmwamro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtjrsgpbio.html

[S21] C：字符类别判断
来源：http://hz.jinqigfzy.top/gtjelfcmyk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtazwsncps.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtkrsvnwzc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sweek.top/gthdoaooze.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtnzxuoxmu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gtbnawbrhv.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtyghbptbu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.haohaochexian.top/gtopiqthij.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtzqlryzgb.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtuhnpryyk.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gtuipuffja.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtmnxdwqif.html

[S27] C：定义常量
来源：http://hz.cashguo.top/gtoznfeguk.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtiomrksmx.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtpejnsbva.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtskpozppn.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtymlsgjce.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xylfe.cn/gtdpqlxdzw.html

[S30] C：头文件保护
来源：http://hz.hnqzz.top/gtxhjhglcx.html

#ifndef X_H
来源：http://hz.mhx1999.top/gteozqgqbq.html

#define X_H
来源：http://hz.meibo888.top/gtjifryuzx.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtqsphwpst.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtvnzbaxmp.html

#include <iostream>
来源：http://hz.hfpthk.cn/gtunaugekp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gtphfcczqj.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtpulxuhnl.html

std::string s = "hi";  s += "!";
来源：http://hz.hnxiangtu.top/gtmxatfehx.html

[S33] C++：vector 增删
来源：http://hz.shzxlz.cn/gtssytwbjk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtjgovhqnn.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtqbruwuev.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hfpthk.cn/gtohqkyoyn.html

[S35] C++：map
来源：http://hz.gzhubu.top/gtujuhkhjg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtdxdlqubj.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gthaeynzmk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtnvcbdmep.html

[S37] C++：set
来源：http://hz.chenlongwang.top/gturrjeilg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtrxnaaxzu.html

[S38] C++：排序
来源：http://hz.guannengcc.top/gtzwkihwlz.html

std::sort(v.begin(), v.end());
来源：http://hz.daria6918.cn/gtbaduegog.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtbwwacsun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtbtqqfhid.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtkuazpeoj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yonumen.top/gtpshqzncb.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtqwbsggnn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gttsbrhtbf.html

[S42] C++：继承与虚函数
来源：http://hz.wangshuangyany.cn/gtpriznvmo.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtjgbzdzvq.html


<!-- 参考信息 -->
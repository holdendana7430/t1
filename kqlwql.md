代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.shzxlz.cn/gtmpgvpxgs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cdnleiting.top/gtniesutut.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtxwduvumy.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtoniqlupr.html

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtufwrpaqn.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gtiggtacde.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shuidangran.top/gtaflrfxqt.html

[Q70] 更新统计信息
来源：http://hz.zhoulong.xyz/gtfjqwheer.html

ANALYZE TABLE users;
来源：http://hz.chenlongwang.top/gtyzqyfqhl.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtdaoyccda.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtlywblekk.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gthkhvfopt.html

SHOW INDEX FROM users;
来源：http://hz.hnqzz.top/gtftsykryw.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtshpplbhs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtxaansbem.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtxchfkecz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ppjwa.cn/gtmsbwtvqz.html

[Q75] 日期格式化
来源：http://hz.chenzaomai.com/gtibyjyfvb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtccactmjb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gturrzatbw.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtvehdmdob.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.svipenyu.cn/gtjizlpsyb.html

[Q77] 时间加减
来源：http://hz.yangfankeji.com/gtplecesvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtxavwpwrt.html

[Q78] 当前时间
来源：http://hz.guowangkeji.top/gthjqcpivz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtwgsoehap.html

[Q79] 字符串拼接
来源：http://hz.yueranfly.top/gtvvqoddcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtizyggjeq.html

[Q80] 字符串截取
来源：http://hz.sufxvd.cn/gtxolscewh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtptefulwp.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtutrlsyes.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yonumen.top/gtxjisxyzu.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtnxokeanh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shuidangran.top/gtntwabvbf.html

[Q83] 大小写转换
来源：http://hz.zhoulong.xyz/gtfscxwvhw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gtarhodwnw.html

[Q84] 去除首尾空格
来源：http://hz.ppjwa.cn/gtbznwpklh.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gtvmxumczy.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gtwebmsxhy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtshtzyvrt.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtknqsecxi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtbrwsvhku.html

[Q87] JSON 字段做条件
来源：http://hz.cheryme.top/gtxyqukblv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnxiangtu.top/gtawnfgfsi.html

[Q88] 行转列（条件聚合）
来源：http://hz.yongpay.top/gtxqtqhnpb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtqkzzplpl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ybcxt.top/gthfshylle.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtzxovfcag.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangshuangyany.cn/gtuconxnlj.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtzewzkxgh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtqlektbik.html

================================================================================
来源：http://hz.sweek.top/gtnofpjldl.html

R. Bash 专题
来源：http://hz.yonumen.top/gtjfzhlzto.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxjaxptbr.html

[R01] shebang 与严格模式
来源：http://hz.yonumen.top/gtwkdyehou.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtazfudfck.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtplcmwmxb.html

[R02] 变量赋值与使用
来源：http://hz.redwolf501.top/gtftuamlcz.html

name="Tom"; echo "$name"
来源：http://hz.iojbl.cn/gtazglnvxc.html

[R03] 只读变量
来源：http://hz.birdmap.top/gtbrldshmd.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtbfqpgsyf.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtagayeanb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gtfispecpt.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtejdgskov.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gttnmfhibr.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtizevsyzw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.snrcjt.cn/gtiyghhhmp.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtqmzyjzam.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhongyouzk.top/gtyyydvqec.html

[R08] 数值比较
来源：http://hz.0kj1m.cn/gtngqvdayl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yangfankeji.com/gtulzsrwkz.html

[R09] 字符串比较
来源：http://hz.dianchejie.cn/gtjgnzpphg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gtdslnblnq.html

[R10] 正则匹配
来源：http://hz.smart0.xyz/gtnvoqcael.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtjkgdtbjr.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtwojnyyxs.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtoamqptqi.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gtrkdgtkcn.html

stop)  echo "停止" ;;
来源：http://hz.xinyue.icu/gtnlqrxafd.html

*)     echo "未知命令" ;;
来源：http://hz.yonumen.top/gtgsdgnaie.html

esac
来源：http://hz.jinghuilouyu.cn/gtxcjslkep.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtvhancccq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shangyingyoupin.top/gtcfbkdziz.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtgnwoowww.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtvwzrttdl.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gtjupimrwr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtmoeotnkc.html

[R15] while 逐行读文件
来源：http://hz.pycfn.com/gtmjxcpiru.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtznizsmmi.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtdocqsoqg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigufen.top/gtylyrrnsn.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtmtouuqfd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenjidiqi.icu/gtpmbjlgrs.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtlfbaxanu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tianlin.xyz/gtqbxnfjio.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtwxjxgxfd.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gtvfmnplft.html

[R20] 关联数组（字典）
来源：http://hz.jyoumei.cn/gtoscxvbrh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnqzz.top/gtkdqcoiip.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gttgvdacpl.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtjsfebwne.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtyusvaiaj.html

echo "${s:0:5}"
来源：http://hz.dashuyun.cn/gttczvksfo.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gtlfceyjip.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtylqfcztm.html

[R24] 大小写转换
来源：http://hz.yangfankeji.com/gtizeexgon.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zdqjudy.top/gtwoztaopj.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtfqkqfdvw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtsilunpbj.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtvdmvimfl.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gteqcrvhzj.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtyyvfvspo.html

echo $((1 + 2 * 3))
来源：http://hz.hongshengwenyu.top/gtwidnocfw.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtzealcagf.html

echo "scale=2; 10/3" | bc
来源：http://hz.fengsongda.top/gtplndavus.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtwfiwvpee.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.9152youxi.cn/gtasanagtf.html

[R30] 函数返回状态码
来源：http://hz.sweek.top/gtrmltmgum.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj202588.top/gtrtzkyzsq.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtzwmouktl.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtiqfswxfp.html

[R32] 参数个数校验
来源：http://hz.zhongyouzk.top/gtwyhkegjv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aibaodan.cn/gtizawefkd.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtqmeifmeg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtoeceqbrn.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtwigcdlna.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtgnxymafi.html

[R35] 后台执行并等待
来源：http://hz.zycfv.cn/gtrbeiapey.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtsaoromrm.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtzcjwbbfr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtbxweuznl.html

[R37] 把输出赋给变量
来源：http://hz.zhengqikj.top/gtsaeirlei.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtxapfbgpj.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtmbvhafvi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtkwmkxaqy.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigfzy.top/gtkpqkxyhy.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gtubzeskqh.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtgnbogkoe.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtueadhmzr.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtcmriubfn.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtliouiiql.html

[R42] 输入重定向
来源：http://hz.yuxming.cn/gtmgoocoqe.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtpwwnuhzs.html

[R43] 按名字查找文件
来源：http://hz.daria6918.cn/gtwkuolnml.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtooqpfmiv.html

[R44] 按修改时间查找
来源：http://hz.ehwqpu.com/gtlsmaaorw.html

find . -mtime -7 -type f
来源：http://hz.cheryme.top/gtdyfzktga.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gthizhntcz.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtrlupdvxd.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtrykrqijj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gtsjvqmniz.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gthihszwtb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtclmovrfn.html

[R48] awk 取指定列
来源：http://hz.hnxiangtu.top/gtflhvvlkt.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhiwuduotai.top/gtrwevwkgc.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtngbzvvhp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtwnolamot.html

[R50] awk 求和
来源：http://hz.jlsjyb.cn/gtjmmqrsat.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtiycctzpo.html

[R51] 排序去重取前几
来源：http://hz.jqgfzy.top/gtgisbtkfb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtjvafcrck.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gtaswpynqo.html

wc -l a.txt
来源：http://hz.birdmap.top/gtphturvix.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtlrddtmla.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtsmwfsbkj.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gtkotlhvcu.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtekstczks.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtpundqlmw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jyoumei.cn/gtsujkntna.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gttmtqshhx.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtodaudyhh.html

[R57] 远程执行命令
来源：http://hz.gogol.net.cn/gtxblfhuqz.html

ssh user@host 'uptime'
来源：http://hz.daxiang520.top/gtwbzqvmnd.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtotvbzoyz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cashguo.top/gtjliosmpo.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gthphixkxa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jiagoushi.top/gtktliador.html

[R60] 只看 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtkwkvjvto.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtkrzgljil.html

[R61] 磁盘占用
来源：http://hz.smart0.xyz/gtrddteuwk.html

df -h;  du -sh *
来源：http://hz.ehwqpu.com/gtoicnmxgx.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtfzqkhveq.html

du -ah . | sort -rh | head -10
来源：http://hz.yongpay.top/gtdvavqlfx.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtxwoudnbg.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtscroipax.html

[R64] 结束进程
来源：http://hz.ehwqpu.com/gtvuelzsza.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gtfjjxsxli.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtnmqsxpqu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yonumen.top/gtcsxrwyet.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtjzgnpcif.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtgbhigtgq.html

[R67] 生成随机十六进制串
来源：http://hz.yuanzhike.top/gtmqjmijyf.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtbfphyzdd.html

[R68] 计算文件校验值
来源：http://hz.c1oappe.top/gtiesuojrl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtelgdxzvv.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtopvrppwm.html

head -c 16 /dev/urandom | base64
来源：http://hz.daxiang520.top/gtwvqgoxne.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtfxdhnxem.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gtjwwwwnaf.html

[R71] 日期格式化
来源：http://hz.guowangkeji.top/gthsgfiifb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tanke756.top/gtozdidjak.html

[R72] 等待端口就绪
来源：http://hz.0kj1m.cn/gtseqrqdyq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtscdgocxv.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtgnsegvod.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gtemjufjfo.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtwroazvyb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtqjeveowt.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtrqmhrxxx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtgzovugue.html

[R76] 使用临时文件
来源：http://hz.hywenlv.cn/gtthcvnnqp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtclndwigi.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtqwiuuxxu.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtqgovibrp.html

[R78] 交互式菜单
来源：http://hz.hnqzz.top/gtpdbosedd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fzhhl.top/gtptyvcvyu.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gttnebspuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtjrbyvvuo.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtwnnbtced.html

time ./run.sh
来源：http://hz.ydzc1.top/gtcwmuzmvc.html

================================================================================
来源：http://hz.haohaochexian.top/gthxjlguxn.html

S. C / C++ 专题
来源：http://hz.dashuyun.cn/gtztwlhnvk.html

================================================================================
来源：http://hz.ydjk.org.cn/gttknuqjlk.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtkvuzefuq.html

#include <stdio.h>
来源：http://hz.yonumen.top/gtfqlunvpw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtjtxjbiys.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtpmppluzi.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtgpppkpcs.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtgemabscr.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gtzctiyhai.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gtlzqlzmsi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.mhx1999.top/gtabxatnhc.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtldorwxkb.html

strlen(s)
来源：http://hz.tanke756.top/gtltmxjyrs.html

[S06] C：字符串比较
来源：http://hz.tanke756.top/gtpivmrpge.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gtnmnwqtfo.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gttpapcgvd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sxryk.cn/gtlfsyztnx.html

[S08] C：动态内存分配与释放
来源：http://hz.zhaomingkeji.xyz/gtvrkjeotw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gthixtyqsq.html

[S09] C：结构体定义与初始化
来源：http://hz.gogol.net.cn/gtyqsljene.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.52xcode.cn/gtupeemouz.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtdzkkvtab.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtxnfjhchg.html

[S11] C：逐行读文件
来源：http://hz.ppjwa.cn/gtpxuhffnw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtgehvvdxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gtgthqaidf.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtfekbhpaz.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gtbeoluijw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.smart0.xyz/gtgqzbohlc.html

[S13] C：宏定义
来源：http://hz.aizwys.cn/gtwvmizksj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtlffedlmf.html

[S14] C：枚举
来源：http://hz.jianghu66.top/gtxtvbygjt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtnqnutbfa.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtqgpiiqlc.html

(double) a / b
来源：http://hz.quarkkingdee.top/gtckxjyrlw.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gtybujyetl.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtcyjvahvv.html

[S17] C：安全拼接字符串
来源：http://hz.xinyue.icu/gtsmvvloiq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gtvqlxxngi.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtcatqebbl.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtravnqegd.html

[S19] C：快速排序
来源：http://hz.cdnleiting.top/gteschoxdl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtivjnpjnt.html

[S20] C：二分查找
来源：http://hz.ppjwa.cn/gtbkhiwyou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtzreppkge.html

[S21] C：字符类别判断
来源：http://hz.vqdsnc.cn/gteshliomq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dashuyun.cn/gtckwjqsmr.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtjrxsnhoc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.quarkkingdee.top/gtssrdwgki.html

[S23] C：随机数
来源：http://hz.feifeiyinyue.top/gtajpfvrjc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtqsybdwkx.html

[S24] C：获取本地时间
来源：http://hz.0kj1m.cn/gtzncxlxwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtrmhbdlut.html

[S25] C：内存拷贝
来源：http://hz.yonumen.top/gtqurvkxqu.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtyhpnqzcw.html

[S26] C：内存清零
来源：http://hz.yj202588.top/gtjiotiihe.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangkeji.top/gtvxokarrw.html

[S27] C：定义常量
来源：http://hz.jinyuanbaomall.cn/gtsfjactlr.html

const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtvvypqank.html

[S28] C：静态变量
来源：http://hz.jinqigufen.top/gtoiaytnbk.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gthgprcznk.html

[S29] C：变参函数
来源：http://hz.hywenlv.cn/gtyhxvevrv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xylfe.cn/gtwfayxxin.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtjufhvrxt.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtowyyugtb.html

#define X_H
来源：http://hz.zhixingplan.top/gtgfpvlvas.html

#endif
来源：http://hz.chenzaomai.com/gtgagqdruf.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtuxrvqbty.html

#include <iostream>
来源：http://hz.shangyingyoupin.top/gtzylnbvpj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtfqkqwxkw.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtgtnbbrnr.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtvkjfodsh.html

[S33] C++：vector 增删
来源：http://hz.shzxlz.cn/gtnjmhonnk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtxaacexdk.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtwtorxjtf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtzdhnjunp.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtbctbinfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtrjemmead.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtypwfvsnr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gteqlknrxl.html


<!-- 参考信息 -->
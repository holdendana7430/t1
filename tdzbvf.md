代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cdnleiting.top/gttynavxio.html

[Q58] 累计求和
来源：http://hz.aibaodan.cn/gtmygxaoqj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yueranfly.top/gtpurcbjno.html

[Q59] 分组内累计
来源：http://hz.pengpengdd.cyou/gtlmqjpngr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtygacczjx.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtilknvhsm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtaoiyebgp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtungycrin.html

[Q61] 移动平均
来源：http://hz.gaohongyu789.top/gtorqyqmtd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtywxugqye.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtdgjelnye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtvvxwvzge.html

[Q63] 开启事务
来源：http://hz.yuxming.cn/gtzlnwrjej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ehwqpu.com/gtuadzcjjp.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtpvvrdwyj.html

COMMIT;
来源：http://hz.yongpay.top/gtkovojkok.html

[Q65] 回滚事务
来源：http://hz.jinyuanbaomall.cn/gtdlgencuo.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtnhzhkymg.html

[Q66] 行锁查询
来源：http://hz.sufxvd.cn/gtqxluhzzt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtpztvkwlh.html

[Q67] 设置隔离级别
来源：http://hz.jyoumei.cn/gtnzmbtdfh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gtkjqzcnhg.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtbzdwylqp.html

SAVEPOINT sp1;
来源：http://hz.redwolf501.top/gtcakzrlwm.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtxquasole.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtefwfhfbz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gttaasqlef.html

[Q70] 更新统计信息
来源：http://hz.hfpthk.cn/gttwxvghgi.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gticjubsld.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtiltruqta.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhixingplan.top/gtwgidqhqw.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtyqnycdgg.html

SHOW INDEX FROM users;
来源：http://hz.yangfankeji.com/gthdsgmptl.html

[Q73] 查看表状态
来源：http://hz.nanxuanxn.top/gtwmzydkzj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenlongwang.top/gtzwstchql.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtziqlydli.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gtumctnlqd.html

[Q75] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtpwgvfjcx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuxming.cn/gtlvhxgxnf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.redwolf501.top/gtfrnbpukc.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtvuvgzpbi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxuanxn.top/gtodiuewbq.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtljevezod.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtyrkusxaq.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtonwjhgvf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtrdblxktf.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gtqsvjamxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ybcxt.top/gtcttycsyj.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtrvpxvqtj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.9152youxi.cn/gtkvrhowox.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtbnwprlxk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhaomingkeji.xyz/gtlvdxcdrb.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtmfvnsveq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cashguo.top/gtdjpkxywj.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gtxguujnjq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtvbghrnca.html

[Q84] 去除首尾空格
来源：http://hz.aizwys.cn/gtlljxgtgz.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gtwonatmjc.html

[Q85] 数值取整
来源：http://hz.gaohongyu789.top/gtvjhyjsol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtsgcmydie.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gtmnbcarcz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtjouiatme.html

[Q87] JSON 字段做条件
来源：http://hz.fzhhl.top/gtuheobcng.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xziqi.cn/gtvfruklfo.html

[Q88] 行转列（条件聚合）
来源：http://hz.cqqwz.cn/gtnlgfurux.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtoogjzbbi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gtclbhyxqz.html

[Q89] 判断表是否存在
来源：http://hz.smart0.xyz/gtsogbwlic.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtsjmdcduz.html

[Q90] 生成序号列
来源：http://hz.shuidangran.top/gtqrowsful.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtspieprjg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxsyjxerr.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtglitufpz.html

================================================================================
来源：http://hz.dashuyun.cn/gtxzgmablk.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtreavendl.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtbrphnpyp.html

set -euo pipefail
来源：http://hz.jqgfzy.top/gtzxwbsrhu.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtwxdpffse.html

name="Tom"; echo "$name"
来源：http://hz.xuetiantiany.cn/gtwdvmexfl.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gtvphkjrua.html

readonly PI=3.14
来源：http://hz.ybcxt.top/gtoogytabn.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gtddamguxq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ivvv.top/gtikkaxrzf.html

[R05] 参数默认值
来源：http://hz.dianchejie.cn/gtrgtxarsh.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtrnaptqmc.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtesjxpfwx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtokgehhkq.html

[R07] if 判断文件
来源：http://hz.ydjk.org.cn/gtlvrqgcvc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtyjqbiyvx.html

[R08] 数值比较
来源：http://hz.gzhubu.top/gtrsjrqusz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sysykeji.top/gttrxdnuex.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gtfonytjdo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtgfxceqaf.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtylvpokul.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtiuevjeic.html

[R11] case 多分支
来源：http://hz.ydzc1.top/gtgzrkqwvp.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtzhurbkcd.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtzxbecnul.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtlqhfqzmg.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtffipyize.html

esac
来源：http://hz.shangyingyoupin.top/gtgmawugzv.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtyjyugflb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtwepmubzd.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtvifunpqr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtycfwvvcr.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtpdwopmlo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gtehvxoclh.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtbebxvzyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.316326.xyz/gtpvtxudiu.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtzabextbu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.iojbl.cn/gtrigntkgb.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtmptwbjyr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtjmtyikzt.html

[R18] 遍历数组
来源：http://hz.andypj.xyz/gtragpilaw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhixingplan.top/gtcfuepxfd.html

[R19] 数组长度
来源：http://hz.zhoulong.xyz/gtytjpnkth.html

echo "${#arr[@]}"
来源：http://hz.nanxinkj.top/gtlxqtukpk.html

[R20] 关联数组（字典）
来源：http://hz.nanxuanxn.top/gtusebirdb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtoiakwuvs.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gtuewrpjap.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtzoyykhwn.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gtznlwhlkr.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtzgpkjnxj.html

[R23] 字符串替换
来源：http://hz.zdqjudy.top/gthqgiynwx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtnvzzssjl.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtlygalyvw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yonumen.top/gttnwqpekn.html

[R25] 去后缀 / 去前缀
来源：http://hz.c1oappe.top/gtsmduqyai.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gteitqrqmr.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtuurtazqy.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtijiwrifi.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtwljbltfr.html

echo $((1 + 2 * 3))
来源：http://hz.shuidangran.top/gtgalpcytf.html

[R28] 浮点运算
来源：http://hz.birdmap.top/gtrgeryxat.html

echo "scale=2; 10/3" | bc
来源：http://hz.meibo888.top/gtwpkodssr.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtynyemlmt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtujisriif.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtauqieyjb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuanzhike.top/gtzjpqkzzt.html

[R31] 局部变量
来源：http://hz.yj202588.top/gtkwzfqhnm.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangkeji.top/gtlmocdmqp.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtnhnbixzs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daxiang520.top/gtzppwrnkf.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtkkaeicjm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtrfijtbkq.html

[R34] 退出时清理
来源：http://hz.daxiang520.top/gtzpipoexp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtgjbemwed.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtmkuxhzvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgufenzy.top/gtnfwylkjv.html

[R36] 并发执行多个任务
来源：http://hz.hammf.cn/gtsieieqor.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gtmiosxnso.html

[R37] 把输出赋给变量
来源：http://hz.yuanzhike.top/gtsimasbve.html

files=$(ls -1)
来源：http://hz.nwbrower.top/gtuxyfzocb.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtvhrqdjbg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtaofcazwo.html

[R39] 重定向标准输出与错误
来源：http://hz.c1oappe.top/gttbgoaniy.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtljgaovae.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtkylzsrui.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtybjlfaxk.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtivbsqrte.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtzamhbupj.html

[R42] 输入重定向
来源：http://hz.316326.xyz/gtqzixywji.html

wc -l < a.txt
来源：http://hz.jyoumei.cn/gtmaompcdt.html

[R43] 按名字查找文件
来源：http://hz.chenjidiqi.icu/gtkrnptmcc.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtfvwwmbpp.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gtsmpuoefi.html

find . -mtime -7 -type f
来源：http://hz.shuidangran.top/gtgtfvdysb.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtpfsvfffw.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtrlwhczcr.html

[R46] 递归替换文件内容
来源：http://hz.sxryk.cn/gtnfxedkek.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtbwzrctsf.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gtqlgpvhgo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.snrcjt.cn/gtzpfktnoj.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gtmyguhgph.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtybjyavxy.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gtcindhzng.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gthbazmpri.html

[R50] awk 求和
来源：http://hz.chenzaomai.com/gtzlqewdcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gtigryynqz.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtodzltmgs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gotoacloud.top/gtdhztydjk.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gtpuvowulr.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtbkfrcnln.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtesuicujm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtzcnwfqiw.html

[R54] 比较两个文件
来源：http://hz.yuanzhike.top/gtyuyqrllx.html

diff a.txt b.txt
来源：http://hz.jinyuanbaomall.cn/gtqkmxwxku.html

[R55] 压缩与解压
来源：http://hz.pengpengdd.cyou/gtxonwlfxa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yvedp.cn/gtpllznzcy.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtxhicghqx.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtifjitmyq.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtnhhkpnou.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtrfhjgndw.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtjednxoev.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtlvslyfts.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gthsidiwxu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtkpmszuxu.html

[R60] 只看 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtbafhvwaq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnxiangtu.top/gtuphvujsi.html

[R61] 磁盘占用
来源：http://hz.xziqi.cn/gtqlvqbvmx.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtqrgtsoyw.html

[R62] 找最占空间的文件
来源：http://hz.vqdsnc.cn/gthjpimsul.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtwiqjkevj.html

[R63] 内存与进程
来源：http://hz.havefunace.top/gttsmeucmf.html

free -h;  ps aux | grep nginx
来源：http://hz.shuidangran.top/gtpcbktvny.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtlmevyyzv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydzc1.top/gtrzlhwroo.html

[R65] 查看端口占用
来源：http://hz.9152youxi.cn/gtxtcvzprv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gogol.net.cn/gtlycozfgx.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtqgmvuewq.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtogwieycz.html

[R67] 生成随机十六进制串
来源：http://hz.nanxuanxn.top/gtyelybsnl.html

openssl rand -hex 16
来源：http://hz.ehwqpu.com/gtntpoffdx.html

[R68] 计算文件校验值
来源：http://hz.andypj.xyz/gtolpeynfq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtyznarvbq.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtiwgjttti.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtyonbkvek.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtsuufauaf.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtchpmorrg.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtggrxdrzi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sxryk.cn/gtzzvaidst.html

[R72] 等待端口就绪
来源：http://hz.316326.xyz/gtpetdzydh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtleodvffy.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtxzgtexcg.html

split -l 1000 big.log part_
来源：http://hz.sweek.top/gthrvuwqvz.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtwvatvhia.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtuugyueap.html

[R75] 导出环境变量
来源：http://hz.xuanzx.com/gthlfsjabh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangkeji.top/gthapqrhat.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtmcqucmgv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtastexhwz.html

[R77] 读取用户输入
来源：http://hz.sufxvd.cn/gtluencjlo.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gterhyzqdo.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gtaxdaepzc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gtwyqlozmd.html

[R79] 解析命令行选项
来源：http://hz.meibo888.top/gtrlxjlczl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.bjfxy.top/gtczbhradp.html

[R80] 查看脚本执行耗时
来源：http://hz.jianghu66.top/gtuvljudpq.html

time ./run.sh
来源：http://hz.cucudq.cn/gtuloegjet.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjqawotyj.html

S. C / C++ 专题
来源：http://hz.shzxlz.cn/gtvncikqxd.html

================================================================================
来源：http://hz.hywenlv.cn/gtwidmszbb.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtarkwqycx.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gtjklwgmml.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shangyingyoupin.top/gtafgunlon.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtltrzhwsg.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gthoivubrc.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtvcklxeqi.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gtdpztvvxb.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtqgcvjuix.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gtfcyzvirv.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtyprgcags.html

strlen(s)
来源：http://hz.shuidangran.top/gtftzhasqv.html

[S06] C：字符串比较
来源：http://hz.yvedp.cn/gtstzlfswk.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtwutiudcs.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gthqpwlomy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daria6918.cn/gtlplrckdo.html

[S08] C：动态内存分配与释放
来源：http://hz.kuanghao11.cn/gtdrsdpory.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gtmvxuwfin.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtuzqdxavn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtooxbauyh.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtuzllmstw.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtkgzwrbfw.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtaspykyxk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhengqikj.top/gtetcastkz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fengsongda.top/gtxdmdmdbz.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gthfieqipa.html

[S12] C：写文件
来源：http://hz.jinqigufen.top/gtefsuxlvh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gttszqayhz.html

[S13] C：宏定义
来源：http://hz.svipenyu.cn/gtubdlvgvm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hongshengwenyu.top/gtadkahuid.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtnomxvfvb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gtwvhdecpq.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtbicmgjdh.html

(double) a / b
来源：http://hz.hammf.cn/gtsebkergy.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gthyrqziue.html

x |= (1 << 3);
来源：http://hz.nanxinkj.top/gtbqsanysi.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtjbaduibv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gtecpfoszt.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtonirfiec.html

int main(int argc, char **argv)
来源：http://hz.yuxming.cn/gtkkhjeqvf.html

[S19] C：快速排序
来源：http://hz.nanxinkj.top/gtmleuctqh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtdnonqiwg.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gtrmmuwtxo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtuynyrjex.html

[S21] C：字符类别判断
来源：http://hz.cdnleiting.top/gtjomrktbd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yangfankeji.com/gtnvmjwqwk.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gtaumcaoss.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtfaztriox.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gtfbupnkcw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tanke756.top/gtmjbunluh.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtvvuffscq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtkhjkxhzn.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtxlynrysv.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtvgcclwkd.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtbnjbcmdv.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtadeguyvj.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtjhfmcbgx.html

const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtiifkexqt.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gthtzrqnte.html


<!-- 参考信息 -->
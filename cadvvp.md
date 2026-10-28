代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhixingplan.top/gtivzmelsv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.haohaochexian.top/gtawzhrteo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.smart0.xyz/gtvxaxgwil.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtlmvoxwkf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jiagoushi.top/gtrrvkiyrs.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtrdjtcptz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xylfe.cn/gtwpudyfdq.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtugfcsvgj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yongpay.top/gtgghhfuyq.html

[Q60] 取上一行 / 下一行
来源：http://hz.gaohongyu789.top/gtpxzrbxeq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtnmgppjhs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guannengcc.top/gtfzerbcdj.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtdxudpuys.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gogol.net.cn/gttpuekguy.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtbntmawjd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtejqhwpzi.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gthyxdgvog.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtcbrulvwp.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtaqwcsskq.html

COMMIT;
来源：http://hz.ehwqpu.com/gtyanxuaoj.html

[Q65] 回滚事务
来源：http://hz.andypj.xyz/gtrjoylrge.html

ROLLBACK;
来源：http://hz.ydjk.org.cn/gtqabxtojr.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtwjlkmhwu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtccfvvagi.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gtdepptaug.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtxtgokiqj.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtcrqocznb.html

SAVEPOINT sp1;
来源：http://hz.jinghuilouyu.cn/gtyytjekmj.html

ROLLBACK TO sp1;
来源：http://hz.yanxiufei.cn/gtjpcfenyi.html

[Q69] 查看执行计划
来源：http://hz.xuetiantiany.cn/gtvsrrneqi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gtjwgoqcvs.html

[Q70] 更新统计信息
来源：http://hz.sufxvd.cn/gtwrkclsee.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtsgiazmav.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtuggagvoa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jlsjyb.cn/gthmlhprid.html

[Q72] 查看索引
来源：http://hz.kuanghao11.cn/gtoppvlqze.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtceovnbod.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gtdplqlqxn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuxming.cn/gthuxsvuxa.html

[Q74] 强制使用索引
来源：http://hz.zhoulong.xyz/gtublxckgv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cheryme.top/gtyeelqqdg.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtmrwfpolo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ehwqpu.com/gthduqvohm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zycfv.cn/gtzargpkkd.html

[Q76] 按天统计
来源：http://hz.svipenyu.cn/gteogrsldl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dianchejie.cn/gtgvftnxuq.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtttqcdmuu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhongyouzk.top/gtvkzlyzgn.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtngqeloqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigfzy.top/gtpoispuuj.html

[Q79] 字符串拼接
来源：http://hz.jqgfzy.top/gtwqxtjjtc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtyqictqoa.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtlloqsiym.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hysaishi.cn/gtapsoflti.html

[Q81] 字符串替换
来源：http://hz.tanke756.top/gtsdajcngi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtxowjlduo.html

[Q82] 字符长度与字节长度
来源：http://hz.zdqjudy.top/gtzeookmnx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtgvmbkebd.html

[Q83] 大小写转换
来源：http://hz.hnqzz.top/gtrbekpoqs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtrwmujcdm.html

[Q84] 去除首尾空格
来源：http://hz.cqqwz.cn/gtgvephvui.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtarkehfxk.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtfactjsjr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shzxlz.cn/gtwagxnjga.html

[Q86] 读取 JSON 字段
来源：http://hz.gotoacloud.top/gtzpacodlm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtqwwfefdc.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtbrjsosgd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtakibonsw.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtmnemwhtk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtrgksksmv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtlbiqgknq.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtjinukuir.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.iojbl.cn/gtzpcaeaxj.html

[Q90] 生成序号列
来源：http://hz.yj202588.top/gtjigollwr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtxvlvpery.html

================================================================================
来源：http://hz.hnqzz.top/gtjqyxcmzw.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtrdkxjkpo.html

================================================================================
来源：http://hz.nanxinkj.top/gtrnxlsmey.html

[R01] shebang 与严格模式
来源：http://hz.yonumen.top/gtdivsmtjs.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangkeji.top/gtgxqmwdub.html

set -euo pipefail
来源：http://hz.yj202588.top/gtdnyuozwx.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gteziperxe.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtzepfdlqb.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtxpeqaqms.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtouquoaza.html

[R04] 位置参数
来源：http://hz.yj202588.top/gtgdkzjhya.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydzc1.top/gtbgvnogdu.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtsxlinnxv.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gteobemtru.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtrrteqzow.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtjipiwfkz.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gtiskodatj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtykqegldq.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtasrievjr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gtqiknkkmy.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtfazjzxag.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtqwoiafqe.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtynixykdx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenjidiqi.icu/gttmgkbjfs.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtcjnatuya.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtpxbpubbn.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtqdzppjoa.html

stop)  echo "停止" ;;
来源：http://hz.cqqwz.cn/gtpjardtbz.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gtdehndzdd.html

esac
来源：http://hz.cashguo.top/gtkvtoxovc.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtzbgicrjp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtwzedewrl.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gthuklrhhv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnqzz.top/gtyhblxytp.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtldbayvnj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yvedp.cn/gtbjpzxavh.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gtktukvvyr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnqzz.top/gtniankjsi.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtpusoxvaa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gtykqodbur.html

[R17] 数组定义与取值
来源：http://hz.jqgfzy.top/gteehzbvvq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jyoumei.cn/gtwbqreahx.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtmxrrnpcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jyoumei.cn/gtcsjqgkjt.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtsxjtngbp.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtbchsjepn.html

[R20] 关联数组（字典）
来源：http://hz.daria6918.cn/gtmeokbjpw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gtlhtfulbi.html

[R21] 字符串长度
来源：http://hz.chenzaomai.com/gtuvojbvvv.html

echo "${#s}"
来源：http://hz.tanke756.top/gtvfniymzc.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtnyxtydvb.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gttvnzxrrx.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtguosuacn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gthikvsvxd.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtulwidygk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.redwolf501.top/gtdpjuksvm.html

[R25] 去后缀 / 去前缀
来源：http://hz.jyoumei.cn/gtgbioweed.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fengsongda.top/gtcytdiynk.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtsqkgblgl.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtyfydmixm.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtalfnstir.html

echo $((1 + 2 * 3))
来源：http://hz.zhiwuduotai.top/gtpwhbkoxe.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtnzqospdi.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtdnxnylrd.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtzkfnfimz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xylfe.cn/gtochauugt.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gttqspqcae.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gttawvxant.html

[R31] 局部变量
来源：http://hz.cashguo.top/gtngfrzgbd.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtqbkjmofy.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtdhnswnju.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtlpptwovm.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gtuqfapugp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhiwuduotai.top/gtuunyuwyi.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gttloazbbu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtdzskxwvl.html

[R35] 后台执行并等待
来源：http://hz.jinyuanbaomall.cn/gtehawmobz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daria6918.cn/gtdqeowrys.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtoivleuoa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.iojbl.cn/gtlmasigyb.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtwiupjrcj.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtvqwgthfa.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtqiqtdgss.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtgdrrduvj.html

[R39] 重定向标准输出与错误
来源：http://hz.aizwys.cn/gtxenbxwvj.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtowfbszar.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtnoapozaa.html

echo "log" >> out.log
来源：http://hz.dashuyun.cn/gtjeasskho.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gttblveenz.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtlvyhezwa.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtdmudynkp.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtggdjyxep.html

[R43] 按名字查找文件
来源：http://hz.xuetiantiany.cn/gtmcbjlmch.html

find . -name "*.log" -type f
来源：http://hz.aibaodan.cn/gtwnjnfeyc.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gttokrhuce.html

find . -mtime -7 -type f
来源：http://hz.svipenyu.cn/gtrhryiwta.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtgctmemke.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtpnnscbry.html

[R46] 递归替换文件内容
来源：http://hz.yuanzhike.top/gtpkvkekml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtsctpubji.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtucfbnabq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.52xcode.cn/gtdpqkffcf.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtercuiwpu.html

awk '{print $1, $3}' a.txt
来源：http://hz.fzhhl.top/gtolvdmcaa.html

[R49] awk 带条件
来源：http://hz.jinqigufen.top/gtltaoxlyo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtfwiwmdef.html

[R50] awk 求和
来源：http://hz.guannengcc.top/gtwqndjksr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.c1oappe.top/gtcpcsgnag.html

[R51] 排序去重取前几
来源：http://hz.316326.xyz/gtaimsbzzy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sweek.top/gtlrltfoju.html

[R52] 统计行数
来源：http://hz.snrcjt.cn/gteoxjunmb.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gthrlcjiso.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtckhiriyo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.c1oappe.top/gtizeuczvg.html

[R54] 比较两个文件
来源：http://hz.jqgfzy.top/gtqbtvtokc.html

diff a.txt b.txt
来源：http://hz.pengpengdd.cyou/gteczhrxfy.html

[R55] 压缩与解压
来源：http://hz.316326.xyz/gtehsxoqjk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtlveuxzcn.html

[R56] 远程拷贝
来源：http://hz.ivvv.top/gtgvsmnecf.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtnczidxvu.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gthcjgfvvn.html

ssh user@host 'uptime'
来源：http://hz.316326.xyz/gtijozcsxe.html

[R58] 下载文件
来源：http://hz.jinqigufen.top/gtcthvupay.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtcsufsmbs.html

[R59] 发 POST JSON
来源：http://hz.yongpay.top/gtwwyjrbxm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fzhhl.top/gtwrestwyo.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtefaxkhjj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenjidiqi.icu/gtevqeecxn.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtzxtxzqft.html

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gtrrnxjzuz.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gtqwoawyml.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtztfgidzb.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtszegtizh.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtfehnfidi.html

[R64] 结束进程
来源：http://hz.zhoulong.xyz/gtqwryldvd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sysykeji.top/gtwiexpqhl.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtpdxrytgm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtrsybjbvz.html

[R66] 定时任务
来源：http://hz.chenjidiqi.icu/gtitbelprr.html

crontab -e;  crontab -l
来源：http://hz.guannengcc.top/gtiqwbqctr.html

[R67] 生成随机十六进制串
来源：http://hz.xuetiantiany.cn/gtzehcrybg.html

openssl rand -hex 16
来源：http://hz.ywan-chungtsiang.top/gtstpawhtl.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gteikkffsl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtblclahdl.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gtzrswiqcl.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtevnsltdr.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtmmblnjwk.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtzpuuaijh.html

[R71] 日期格式化
来源：http://hz.yuxming.cn/gtgwulihuo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj202588.top/gtzsekvmht.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtnkqeiopo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtdigybodr.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtedkcpkcb.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gthfzhbmvk.html

[R74] 批量重命名
来源：http://hz.snrcjt.cn/gtarewqssg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtxcpnntua.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtigzmeejo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gtvcsqzyie.html

[R76] 使用临时文件
来源：http://hz.snrcjt.cn/gtwctoiqmi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtvaerplsc.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtxygvfdhx.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtckjbdwtn.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gtuslzfvsv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangshuangyany.cn/gtegiabjrj.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gtvbapjief.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zycfv.cn/gtqwpkwthx.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtcfnzevql.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gtrgfeywhv.html

================================================================================
来源：http://hz.gotoacloud.top/gtyunshbld.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gtqwyehygb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtroufuhxl.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtwnlsyzez.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtkqmvcnvy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.9152youxi.cn/gtssbmtcjs.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtsrusidsq.html

int a = 10; printf("%d\n", a);
来源：http://hz.guannengcc.top/gtrmzykslj.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gtqdtuovvh.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtfaczdazw.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtuvhiyboq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.birdmap.top/gtsezakdfr.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gthvbbrcgy.html

strlen(s)
来源：http://hz.jianghu66.top/gtisebynqh.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtvagxxwps.html

strcmp(a, b) == 0
来源：http://hz.zhijiandao.cn/gtfgwnixxl.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gtljqzrzxl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.bjfxy.top/gtgknecgxf.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtauywmalb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nwbrower.top/gttxipvvax.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtuukerlxw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tianlin.xyz/gtikokpyoe.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtkiueslps.html

int *p = &a;  *p = 5;
来源：http://hz.yvedp.cn/gtlezogdrk.html

[S11] C：逐行读文件
来源：http://hz.zhijiandao.cn/gtcwhzeugv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.svipenyu.cn/gtuzmclnuq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gttbdwotbc.html

fclose(f);
来源：http://hz.guowangkeji.top/gtpbhwmsuk.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtguqkunej.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sweek.top/gtksrznlnr.html

[S13] C：宏定义
来源：http://hz.cqqwz.cn/gtjgvupyxu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj202588.top/gtuhlocchr.html

[S14] C：枚举
来源：http://hz.jianghu66.top/gtwxlsmusr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtbntgprzg.html

[S15] C：类型转换
来源：http://hz.cqqwz.cn/gtjbzbxxbi.html

(double) a / b
来源：http://hz.yuanzhike.top/gtrkaawrkn.html

[S16] C：位操作置位
来源：http://hz.smart0.xyz/gtcsgrorqo.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtvtitjrtc.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtddugjolf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtflacwyum.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtltqcybyy.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtojhqpzqv.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtpkccamzf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtzgxeejqk.html

[S20] C：二分查找
来源：http://hz.svipenyu.cn/gtermgwidi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtdaboqbxe.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gtvfrpubyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinghuilouyu.cn/gtdtlbsgao.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gthdzqpmfi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtowwwdpto.html

[S23] C：随机数
来源：http://hz.cqqwz.cn/gtqaxqrkmb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gtnmfjwung.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gthejeyhje.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xziqi.cn/gtuhkkznax.html

[S25] C：内存拷贝
来源：http://hz.ybcxt.top/gttqrzmujh.html

memcpy(dst, src, n);
来源：http://hz.smart0.xyz/gtfryjxwtn.html

[S26] C：内存清零
来源：http://hz.jqgufenzy.top/gtcernypfv.html


<!-- 参考信息 -->
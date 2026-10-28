代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuetiantiany.cn/gtsecjbaib.html

[Q60] 取上一行 / 下一行
来源：http://hz.yongpay.top/gtpgzjfrta.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pycfn.com/gtejscastc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtonfkupxo.html

[Q61] 移动平均
来源：http://hz.xuetiantiany.cn/gtpwcvisjc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhongyouzk.top/gtzfzxbuor.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gtmhvyndmg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtpxsklmfs.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gthskfgmra.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtmkgeiccb.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtviatqfpm.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gthdosyqtt.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtqxxasurz.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtegtomgaz.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gtvvztwaop.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtnlgbzbne.html

[Q67] 设置隔离级别
来源：http://hz.shuidangran.top/gtsdoztgpr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.9152youxi.cn/gtdhlwhwgw.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtqwajoxms.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gthcrijait.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gtwggtrwqr.html

[Q69] 查看执行计划
来源：http://hz.birdmap.top/gteanijcew.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtlclibhsu.html

[Q70] 更新统计信息
来源：http://hz.shuidangran.top/gtzzksmlfp.html

ANALYZE TABLE users;
来源：http://hz.52xcode.cn/gtnwkpmoip.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtxmaxcfmw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gtyloefumw.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtxfzacfsl.html

SHOW INDEX FROM users;
来源：http://hz.gzhubu.top/gtgwbhduco.html

[Q73] 查看表状态
来源：http://hz.xylfe.cn/gtqgvmnymz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtyzmljdpg.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtdlrzdjgt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cashguo.top/gtuwxfjfzy.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtszcorvny.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jianghu66.top/gtjgojlmbh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtljprauyq.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtsfbqnjgh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gttcnddxfa.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtstipjjls.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtwyoawnjl.html

[Q78] 当前时间
来源：http://hz.yj20258888.top/gtvnxzfjak.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtkvdvqdqw.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtxvixuvpa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtvuymdjql.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gttyezbopg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtvstqssfk.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtinuwjklp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhongyouzk.top/gtavbeaduj.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtwepzpnop.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtehjqjkan.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtdujmtorj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ybcxt.top/gthbbullhl.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtffzgddcn.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtgqwwskag.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtgzjcveek.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yongpay.top/gtbfjqaven.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtjpdsynob.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtwbkacpjf.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtyznsndcq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.quarkkingdee.top/gtqbqshqos.html

[Q88] 行转列（条件聚合）
来源：http://hz.bjfxy.top/gtlbqgento.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtrcgybdef.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtqldkqwyu.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtjuhlvgbw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xylfe.cn/gtjdeersct.html

[Q90] 生成序号列
来源：http://hz.hnqzz.top/gtnifdfhef.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.feifeiyinyue.top/gtofcpzecn.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvevuipne.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtijxpmiln.html

================================================================================
来源：http://hz.havefunace.top/gtqsdziwoh.html

[R01] shebang 与严格模式
来源：http://hz.mhx1999.top/gtgotzmwbb.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtsoybyrln.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtoasvlszq.html

[R02] 变量赋值与使用
来源：http://hz.wangshuangyany.cn/gtybwyaoyh.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gtmgklfqxf.html

[R03] 只读变量
来源：http://hz.shanyushiyangkeji.top/gtokerayzs.html

readonly PI=3.14
来源：http://hz.gzhubu.top/gtpvvxqrho.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtppzvrtvs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigfzy.top/gtpylxtxxt.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtembbdari.html

name="${1:-default}"
来源：http://hz.xylfe.cn/gtdthgircb.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtbgnbmtko.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtjbphpbnw.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtdeggfvyx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtdouzoyff.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gturtinuct.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtlnjrqtho.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtciqqwdnn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtisqtfcqk.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gtibmldyoc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yangfankeji.com/gtbcjkbduy.html

[R11] case 多分支
来源：http://hz.yanxiufei.cn/gtqshdnioq.html

case "$1" in
来源：http://hz.shzxlz.cn/gtwcaljbiy.html

start) echo "启动" ;;
来源：http://hz.aizwys.cn/gtekurrygj.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtaxbjqzvw.html

*)     echo "未知命令" ;;
来源：http://hz.tianlin.xyz/gtwoyvhqgd.html

esac
来源：http://hz.feifeiyinyue.top/gttsrigvek.html

[R12] for 遍历文件
来源：http://hz.havefunace.top/gtkuzuzcpz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtyrnsqgxz.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtlqwtjnkm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dianchejie.cn/gtxghsperw.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtypecqvts.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtcpujcdej.html

[R15] while 逐行读文件
来源：http://hz.zhongyouzk.top/gtloipxncy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gtsnwgplty.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gtobkajvvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.mhx1999.top/gtzuxcxbxn.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtnrubcfrb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtghbyxscs.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtoqivhxid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtxrpeonyq.html

[R19] 数组长度
来源：http://hz.zhoulong.xyz/gtsuyfnphr.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtrhfjhprb.html

[R20] 关联数组（字典）
来源：http://hz.tianlin.xyz/gtkrllfcuc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtxfqnesnf.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtungdhruz.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtosfrvtfg.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtfalihhdq.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtbsmjqlfv.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtduutzxpk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtpwdmqkue.html

[R24] 大小写转换
来源：http://hz.hysaishi.cn/gtvievwvpu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtvljxiwaq.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtghqdqddh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtyndsxomn.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtkawwqnlj.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gtmgmfnzwh.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtxsiklsra.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtzweasfrm.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtqdgbtmec.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtilxqbwze.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtvxyiltvc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtinkhvfwl.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtqvfjupnt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sysykeji.top/gtagmuvixa.html

[R31] 局部变量
来源：http://hz.ehwqpu.com/gtokwfimwn.html

f() { local x=1; echo "$x"; }
来源：http://hz.andypj.xyz/gtxmhycsis.html

[R32] 参数个数校验
来源：http://hz.cqqwz.cn/gtspwirkek.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.mhx1999.top/gtgediuezi.html

[R33] 捕获错误并提示行号
来源：http://hz.fzhhl.top/gtwrltaulw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtyvobzmfi.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gtlrnokdob.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtenhxqsth.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtbxqlwntg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtogmnbkwk.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gtbzqhvwus.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtgcxenmmf.html

[R37] 把输出赋给变量
来源：http://hz.xingfuxueyuan.xyz/gtuehrvhhn.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtjqisxsyu.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtiayruoey.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gttfmbzywh.html

[R39] 重定向标准输出与错误
来源：http://hz.smart0.xyz/gtsjbkdgvc.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gtpfbqojzx.html

[R40] 追加写日志
来源：http://hz.pycfn.com/gthitmieox.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtifdpgslb.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtsklhxibz.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtqqbkojii.html

[R42] 输入重定向
来源：http://hz.hongshengwenyu.top/gtvjjhxidf.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gttdatohlq.html

[R43] 按名字查找文件
来源：http://hz.cucudq.cn/gtsqlqbwrr.html

find . -name "*.log" -type f
来源：http://hz.xuanzx.com/gtansvzfqr.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtqjipsesn.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtqswssphc.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtdumjxiiz.html

find . -name "*.tmp" -delete
来源：http://hz.nanxinkj.top/gtmktyxydm.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtryhnxluh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtoxxwbztr.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtgsfaqxsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gtpnmtmnfq.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gthpigannu.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtusjbsrzy.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtsrrwfkay.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtudlogahn.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gttoeoyedb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sysykeji.top/gtzlhtetzs.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtlwhqcdbm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtwbgjqqhj.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gthscomcnm.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtdjgiivcy.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtsihobjpi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtpeladdka.html

[R54] 比较两个文件
来源：http://hz.cheryme.top/gtzougkqcv.html

diff a.txt b.txt
来源：http://hz.cheryme.top/gtfsfjwrgi.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtbjzriifg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtyszeenrw.html

[R56] 远程拷贝
来源：http://hz.yonumen.top/gtdqalwher.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtecauazha.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtfnfxpybw.html

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtmhknwtem.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtqmezcklu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtnbnlttgj.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gtfslthqur.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtpalwsgoy.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gteajnxeno.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.havefunace.top/gtskisdkaf.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtotbfmtfd.html

df -h;  du -sh *
来源：http://hz.zycfv.cn/gtylhqreqr.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtwewkzyha.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gtrhsejgsg.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gtvxzzjyhx.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtptcrohes.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtvvvisozw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtszpwnaxo.html

[R65] 查看端口占用
来源：http://hz.wangshuangyany.cn/gtdnykjfhf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhaomingkeji.xyz/gtjaceffbf.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtrcoyxwmx.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtaighowwi.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gtmkwdozwy.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gtoqhobxzl.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gtatugaivx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gtongwdsdk.html

[R69] 生成随机密码
来源：http://hz.yj202588.top/gtsiqzbrli.html

head -c 16 /dev/urandom | base64
来源：http://hz.dashuyun.cn/gtxiubqrgf.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtxokjyxkv.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtmiktiqkt.html

[R71] 日期格式化
来源：http://hz.redwolf501.top/gtbfvuscos.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gtxrmztblv.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gtbacxrxmp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuxming.cn/gtmyonwlzw.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtezyuztzp.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtmtdbxhoh.html

[R74] 批量重命名
来源：http://hz.yuxming.cn/gtksdsqdya.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtehftaoaz.html

[R75] 导出环境变量
来源：http://hz.nanxinkj.top/gtoawqbzop.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guowangkeji.top/gtxfgtodri.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtlaisebcw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gtnscoxmtk.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gtqgexlozu.html

read -rp "请输入: " ans
来源：http://hz.c1oappe.top/gtliakkjbh.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtprcnsvxw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhijiandao.cn/gtbghipgkh.html

[R79] 解析命令行选项
来源：http://hz.jinghuilouyu.cn/gtwmgmfnns.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtbzzyfdak.html

[R80] 查看脚本执行耗时
来源：http://hz.ehwqpu.com/gtjyicmwbm.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtyoqrvaxr.html

================================================================================
来源：http://hz.shzxlz.cn/gtsjayhptd.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtqernashb.html

================================================================================
来源：http://hz.meibo888.top/gttlobzekn.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtdofvzjrd.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtstogotky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtdgdkyewm.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtihwiqsus.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinyuanbaomall.cn/gtpwwpjyyy.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtnytwhgcn.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtgyjfakev.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtwtysfoav.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gttfgggbqz.html

[S05] C：字符串长度
来源：http://hz.hnqzz.top/gtgurulmtw.html

strlen(s)
来源：http://hz.yueranfly.top/gtfegnubcz.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gtkbplrzcc.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtimtkrcut.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtvaubhxih.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.andypj.xyz/gtklbkaafj.html

[S08] C：动态内存分配与释放
来源：http://hz.snrcjt.cn/gtcvswwbfn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gzhubu.top/gtteijuskt.html

[S09] C：结构体定义与初始化
来源：http://hz.tianlin.xyz/gtfturqaob.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtjkxovlza.html

[S10] C：指针与解引用
来源：http://hz.jqgufenzy.top/gtlwagyenr.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtiehplreq.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtwekessev.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtvehclsym.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtebxdgorw.html

fclose(f);
来源：http://hz.xinyue.icu/gtxyrqilkz.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gttnmgdqse.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtuuunfezw.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtjvrbocqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangtech.top/gtfowhjpcb.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtvzldemsp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gtsejwmnbt.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtbvicupod.html

(double) a / b
来源：http://hz.dashuyun.cn/gtcgwvubzz.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtxhffekzh.html

x |= (1 << 3);
来源：http://hz.yvedp.cn/gtlrmxsrbv.html

[S17] C：安全拼接字符串
来源：http://hz.ydzc1.top/gttgovoyct.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtpqvtkxts.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtdhxsliko.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtdfycghmf.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gtpdluikcq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtcwdewthx.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtpcdnlgcc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtcugzxlxw.html

[S21] C：字符类别判断
来源：http://hz.sufxvd.cn/gtqhybkmsr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.havefunace.top/gtcwjvhgba.html

[S22] C：字符串转数字
来源：http://hz.yonumen.top/gtaqjonspz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtscpvimym.html

[S23] C：随机数
来源：http://hz.hywenlv.cn/gtzkcwjxgx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtibrlhrgr.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtuekyxzos.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinyuanbaomall.cn/gtbuzngwjq.html

[S25] C：内存拷贝
来源：http://hz.zhijiandao.cn/gtzzwbdclp.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gtleyykcyu.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtzturcbnn.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtoyzkkqxs.html

[S27] C：定义常量
来源：http://hz.birdmap.top/gtkolnsjpk.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtddawtdne.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtsaaujsek.html

static int counter = 0;
来源：http://hz.gzhubu.top/gtuuqarhai.html

[S29] C：变参函数
来源：http://hz.redwolf501.top/gtaoivsehr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtdgcjxtdq.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtpefbivui.html


<!-- 参考信息 -->
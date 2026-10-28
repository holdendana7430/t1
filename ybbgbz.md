代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtrfnfvuyz.html

[Q50] 批量更新
来源：http://hz.0kj1m.cn/gtrhiudcss.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnqzz.top/gtqeqkxatt.html

[Q51] 用子查询更新
来源：http://hz.jinqigfzy.top/gtvsqhtwvi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jiagoushi.top/gtsgkrfyla.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtyehkbnii.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtyktteeub.html

[Q53] 按条件删除
来源：http://hz.sufxvd.cn/gtitnzsjiq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinghuilouyu.cn/gtupnwfeyz.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtmupwylly.html

TRUNCATE TABLE logs;
来源：http://hz.vqdsnc.cn/gtfilufkyz.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gtqsfihcyb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gttniyfdsd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gtsezpqrvr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtyhtcjrfa.html

[Q57] 行号
来源：http://hz.cheryme.top/gtrzijcotd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hongshengwenyu.top/gtrzjkriwv.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtrkpqxtkr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sysykeji.top/gtdrgxergb.html

[Q59] 分组内累计
来源：http://hz.yangfankeji.com/gtedcogpzr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.meibo888.top/gtzprahuag.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gtdkosddnw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtruxzouaf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xylfe.cn/gtkfacfjqp.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtkoiapfxn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtwnlhjubq.html

[Q62] 分组占比
来源：http://hz.gzhubu.top/gtgsyproga.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtjplsspzv.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtptpsyjcr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.mhx1999.top/gtmbqnmxlw.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtjuxwysmn.html

COMMIT;
来源：http://hz.zhongyouzk.top/gtesdnbpsf.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtoclgpoct.html

ROLLBACK;
来源：http://hz.yj20258888.top/gthsrzfiuz.html

[Q66] 行锁查询
来源：http://hz.shzxlz.cn/gtsjumfbcr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtdzsytets.html

[Q67] 设置隔离级别
来源：http://hz.hammf.cn/gtesagpvxy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtjkhrfrgu.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gtlegimmdm.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtfeqcrzsj.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtrbzdrijx.html

[Q69] 查看执行计划
来源：http://hz.ydjk.org.cn/gtzeltjilg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtszzedium.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gtupmqgumg.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtwxquflir.html

[Q71] 查看建表语句
来源：http://hz.yj20258888.top/gtipiqgdwt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gttlfhnyhf.html

[Q72] 查看索引
来源：http://hz.hywenlv.cn/gtcndzefxy.html

SHOW INDEX FROM users;
来源：http://hz.xinyue.icu/gtkqtxreoa.html

[Q73] 查看表状态
来源：http://hz.gogol.net.cn/gtqvyrewfb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhaomingkeji.xyz/gtukfgeplm.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangkeji.top/gtmnrktqcy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtosypwymz.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtdrztyyia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gttpojjrax.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.haohaochexian.top/gtdlgrspkn.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtixyvvtzd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtkdcuycfe.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gtlhlazmvu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgufenzy.top/gtjbbfqmbk.html

[Q78] 当前时间
来源：http://hz.tian-w.cn/gtrcsmjdmi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtxfqgzzhc.html

[Q79] 字符串拼接
来源：http://hz.yanxiufei.cn/gtnnrqbhgb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhengqikj.top/gtijrtuzva.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtfphzbuef.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258888.top/gtxzkqslhc.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtzxmksvyd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtwhnezyij.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gtrxyjnzhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtibqkjchy.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtlvfyenyy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtarovvcsu.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtralgvzzn.html

SELECT TRIM(name) FROM users;
来源：http://hz.jyoumei.cn/gtuewmvmpy.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtfjlmfalr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhoulong.xyz/gtsuybwtsl.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtfokbdrdu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hammf.cn/gtgizftzth.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtjthkfnqg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gthijqclwd.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gtyedcdmaz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj202588.top/gtxnaddbxy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daria6918.cn/gtqhntaiee.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtjxmpsygp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gtciuksfek.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtbdigoxxe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtctbnyeab.html

================================================================================
来源：http://hz.pycfn.com/gtqeizsjex.html

R. Bash 专题
来源：http://hz.tanke756.top/gtxxtuybyg.html

================================================================================
来源：http://hz.fzhhl.top/gtckimsrqn.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtejivyjww.html

#!/usr/bin/env bash
来源：http://hz.yuanzhike.top/gtrepljjsv.html

set -euo pipefail
来源：http://hz.fengsongda.top/gtjlqhiguk.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtjxwcedgz.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtooinqiar.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtndqqjnvo.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gtmaizzmwe.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtbsnarool.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtgxqjgaeb.html

[R05] 参数默认值
来源：http://hz.gzhubu.top/gttbumstjn.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtonjgokwv.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtqpznvznk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.birdmap.top/gtkdeprxnh.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtnbkosxzx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtwowrgbde.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtpvzkrajf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtwkognzvu.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtnaodrlke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtlhippqln.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtdkpboizj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtjyvwuchz.html

[R11] case 多分支
来源：http://hz.nanxinkj.top/gturdkpyec.html

case "$1" in
来源：http://hz.fengsongda.top/gtewfckwvu.html

start) echo "启动" ;;
来源：http://hz.sufxvd.cn/gtnzjjwmtn.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtmzudfwyd.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gtehiiuslf.html

esac
来源：http://hz.ehwqpu.com/gtlnrcmblq.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtjoqzmaja.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hysaishi.cn/gtpqketbtn.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtvxvzagjq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtclirtafr.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtupyyexzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtvymorfqm.html

[R15] while 逐行读文件
来源：http://hz.yvedp.cn/gtdjcbyfse.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj202588.top/gtiesfiwje.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtnczfgzru.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtkflokndn.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtzkhbzsdb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtwodlyofj.html

[R18] 遍历数组
来源：http://hz.yuxming.cn/gtszalvciu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtnfkdccca.html

[R19] 数组长度
来源：http://hz.vqdsnc.cn/gtpwgijafc.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtuxizeocc.html

[R20] 关联数组（字典）
来源：http://hz.smart0.xyz/gtoosjnvrr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnqzz.top/gtblmlxrsz.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gtvajavqgp.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtkzxsotdj.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtuqwtrfpg.html

echo "${s:0:5}"
来源：http://hz.fzhhl.top/gthlhnfudp.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtpusvyguf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtunqtvhio.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gthexdqfhu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtybhtreht.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtbgmfdvtd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtevwfxiet.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtpvbmrjdc.html

now=$(date +%F); echo "$now"
来源：http://hz.hnqzz.top/gtwrpgdsbi.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtsrjzhflm.html

echo $((1 + 2 * 3))
来源：http://hz.52xcode.cn/gtltpdpsbm.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtuwzmoqud.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuxming.cn/gtxsbjienn.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtnkqgkncd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ywan-chungtsiang.top/gtzodprgzv.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtrrbbdqie.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guowangkeji.top/gtpayzycfn.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtexcsfywa.html

f() { local x=1; echo "$x"; }
来源：http://hz.pycfn.com/gtdakxgzfy.html

[R32] 参数个数校验
来源：http://hz.yuxming.cn/gtdzhkkgsb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtvxnqvjaw.html

[R33] 捕获错误并提示行号
来源：http://hz.iojbl.cn/gtfyfkoffp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.smart0.xyz/gtuehddkxs.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtadxbtmrd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtbnurvwcy.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtznyugybn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtpptpivfv.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtjmbqzthv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtqlrszaur.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtkkeewtwu.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtzfmnfimd.html

[R38] 管道串联
来源：http://hz.yanxiufei.cn/gtybefohec.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sweek.top/gthpaogtmp.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gtdomrmlcv.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtqvuhfacb.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtxeulfnpr.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gtwhivjzba.html

[R41] 丢弃输出
来源：http://hz.yueranfly.top/gtbkyizeac.html

cmd >/dev/null 2>&1
来源：http://hz.cucudq.cn/gtdendtwzx.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gtznoyzkgz.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtrtfkxrnd.html

[R43] 按名字查找文件
来源：http://hz.ppjwa.cn/gtlowoedev.html

find . -name "*.log" -type f
来源：http://hz.zhongyouzk.top/gtcuwfvygq.html

[R44] 按修改时间查找
来源：http://hz.jianghu66.top/gtpugarxcv.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtnhvkqbxs.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gttxrfnjuj.html

find . -name "*.tmp" -delete
来源：http://hz.feifeiyinyue.top/gtwlrxtzto.html

[R46] 递归替换文件内容
来源：http://hz.guowangkeji.top/gttspzkuyl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gteceyinzb.html

[R47] sed 单行替换
来源：http://hz.jinyuanbaomall.cn/gthekpgepc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ivvv.top/gtvxpfxadl.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtochhglrq.html

awk '{print $1, $3}' a.txt
来源：http://hz.hongshengwenyu.top/gtpghnlrlw.html

[R49] awk 带条件
来源：http://hz.316326.xyz/gtbjqkzegl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtkhkpmkkx.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtwssstgre.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.smart0.xyz/gteweoaagt.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtjoovkgxl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.birdmap.top/gttvsjepdg.html

[R52] 统计行数
来源：http://hz.jianghu66.top/gtdwgnfcsn.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gtqrwpeavl.html

[R53] 查看文件头与实时尾
来源：http://hz.jiagoushi.top/gtknfwnngo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydjk.org.cn/gtctxhzxor.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gtahpkjvsk.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtxjgnbfej.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtterywmyu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtljzkroug.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtsckcgrjy.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gttpbwhcrv.html

[R57] 远程执行命令
来源：http://hz.sweek.top/gtxtumpybh.html

ssh user@host 'uptime'
来源：http://hz.cashguo.top/gtvftxjvco.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtrgetzfti.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gteumzfngl.html

[R59] 发 POST JSON
来源：http://hz.aibaodan.cn/gthzryadum.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtfbhwaktg.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtneuuhbic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtoenibcdj.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtdpxxrnsq.html

df -h;  du -sh *
来源：http://hz.guowangkeji.top/gttwnnpcfg.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtwqwzzmke.html

du -ah . | sort -rh | head -10
来源：http://hz.chenlongwang.top/gthtgvhucn.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gtjwrzldlf.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtdjkzbuxc.html

[R64] 结束进程
来源：http://hz.c1oappe.top/gttaqfnrix.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yongpay.top/gtgxdzngzd.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtikhqvjzc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xuanzx.com/gtonrnqesm.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gtslvrihot.html

crontab -e;  crontab -l
来源：http://hz.nwbrower.top/gtgrlpdxzc.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtmerolmld.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtmbmenkap.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtivmccznc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gthsttlbqr.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gtlfqncffk.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gttovhtxlj.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gthwiedqbx.html

date +%s;  date -d @1700000000
来源：http://hz.xingfuxueyuan.xyz/gtkiqqwqnw.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtsqrpxjuh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtbskrdjaa.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtzgvtfsbx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtfmfepbtx.html

[R73] 分割大日志
来源：http://hz.gogol.net.cn/gtuscasrjg.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtbpkgybfg.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gtpptkirde.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgfzy.top/gterqejbrs.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtiwfkmper.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtrpvlmrrl.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtbbwpoczr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtnvuvrxnm.html

[R77] 读取用户输入
来源：http://hz.aizwys.cn/gtkdjofaqt.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtjmzxjpnb.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtwocssojc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gtcxdsyrag.html

[R79] 解析命令行选项
来源：http://hz.xylfe.cn/gtvnerrayj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pengpengdd.cyou/gtznoqegfr.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtfclqfycc.html

time ./run.sh
来源：http://hz.yongpay.top/gtonhmopqc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkcjvvgiw.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtdpziclpb.html

================================================================================
来源：http://hz.yj20258888.top/gtsquwkrdi.html

[S01] C：Hello World
来源：http://hz.kuanghao11.cn/gtyklqbybd.html

#include <stdio.h>
来源：http://hz.xziqi.cn/gtpgfptgen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtqrrgjgcp.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gttyezkpry.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtetddzmvo.html

[S03] C：读入整数
来源：http://hz.ywan-chungtsiang.top/gttzfrhbrw.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtemtkbwtq.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtrvzfsxwb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtmbhpbdrr.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtrcyluvdt.html

strlen(s)
来源：http://hz.havefunace.top/gtenjfthns.html

[S06] C：字符串比较
来源：http://hz.hongshengwenyu.top/gtcudybqqe.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtexxbyyoh.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtizeqmnou.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxuanxn.top/gtixhjsbyd.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtxapbqsjl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tanke756.top/gtghjftjro.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtwrlvjxrt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.svipenyu.cn/gtjrnwbrkl.html

[S10] C：指针与解引用
来源：http://hz.gogol.net.cn/gtoremltfz.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtnmbthasq.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gthljfhkzs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.0kj1m.cn/gtcsrainbx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtgtaigvza.html

fclose(f);
来源：http://hz.ydjk.org.cn/gtumpukxor.html

[S12] C：写文件
来源：http://hz.birdmap.top/gttducsimq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.c1oappe.top/gtccdfjkjo.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtjcrininh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhengqikj.top/gtepydnvnd.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtvpxfoudh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtxoffvddz.html

[S15] C：类型转换
来源：http://hz.jqgfzy.top/gtazldhzuw.html

(double) a / b
来源：http://hz.316326.xyz/gtaaqwwevi.html

[S16] C：位操作置位
来源：http://hz.yongpay.top/gtcsungufa.html

x |= (1 << 3);
来源：http://hz.ppjwa.cn/gtmkttphqq.html

[S17] C：安全拼接字符串
来源：http://hz.zhiwuduotai.top/gtkhdshoir.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangtech.top/gtyozouarg.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtsokebxnd.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtjdlqsfhm.html

[S19] C：快速排序
来源：http://hz.yangfankeji.com/gtucyucrbl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtuvtowftd.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gthasbnzwo.html


<!-- 参考信息 -->
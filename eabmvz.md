代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtymickaqt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtdcgoovur.html

[Q47] 与平均值比较
来源：http://hz.cashguo.top/gthffvrocf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtqntevwrw.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gtvdafnaug.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.9152youxi.cn/gtsfiaambe.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zdqjudy.top/gtpllhwggv.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gteidzwjkd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtdmziisii.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtdzyjdlri.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aizwys.cn/gtiwgtzobr.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gttphbjxxh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtztmuacuf.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtaqlyijkp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.havefunace.top/gtbvsbveeb.html

[Q53] 按条件删除
来源：http://hz.hongshengwenyu.top/gtoruqexms.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gttlulgngk.html

[Q54] 清空表
来源：http://hz.jiagoushi.top/gtcuxqrwqv.html

TRUNCATE TABLE logs;
来源：http://hz.jlsjyb.cn/gtydutuevd.html

[Q55] 排名（并列占位）
来源：http://hz.xziqi.cn/gtokurjemu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gtpwtydnmi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtfitsngwk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xingfuxueyuan.xyz/gtipbpphqy.html

[Q57] 行号
来源：http://hz.jqgfzy.top/gtgllnfqbm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guowangkeji.top/gtalafcndg.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gttklszzot.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yangfankeji.com/gtjamyuizq.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtiuhejibl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtnafxywbg.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gtodgyktus.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gtfanjfrzz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gthnwmoxzo.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gteyxdlxry.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnqzz.top/gtvakqwsbf.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gtarsevqhh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtuhvgmcpr.html

[Q63] 开启事务
来源：http://hz.cucudq.cn/gtpwjjhsae.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtdyxpezkp.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtpynprobt.html

COMMIT;
来源：http://hz.yvedp.cn/gtvirgjguc.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gthyfdeacu.html

ROLLBACK;
来源：http://hz.yuxming.cn/gthcxqqgvx.html

[Q66] 行锁查询
来源：http://hz.c1oappe.top/gtiexsejkb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.iojbl.cn/gtxcodvcyw.html

[Q67] 设置隔离级别
来源：http://hz.smart0.xyz/gtflurfwwe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.kuanghao11.cn/gtnftiqnpt.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtvihazrte.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtklhmdyup.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtohwrdccp.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gtfxzeejlk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinghuilouyu.cn/gtnupityts.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gteubwkjgr.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtomcfrklq.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtspuvtmjx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ehwqpu.com/gtbbnvuepg.html

[Q72] 查看索引
来源：http://hz.guannengcc.top/gteeosiyek.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtvirirglg.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtqyxjlwvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shzxlz.cn/gttcrycvni.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gtmxsoprnc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtxopdqdnr.html

[Q75] 日期格式化
来源：http://hz.pycfn.com/gtyvouqdcg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtgfrvbyys.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fzhhl.top/gtfcjnuyze.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gtxkvrvbdo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxuanxn.top/gtxbmkjjsw.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtahglznxh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtpvvuwpid.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gtdryztkyy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtteutogmc.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gtmbrsnxuy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yonumen.top/gtpynjkbyd.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtdmnslujm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtamqokpuj.html

[Q81] 字符串替换
来源：http://hz.chenjidiqi.icu/gtykpehwaa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtjdjpseru.html

[Q82] 字符长度与字节长度
来源：http://hz.shzxlz.cn/gtniqfvppl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sysykeji.top/gtmuywsawj.html

[Q83] 大小写转换
来源：http://hz.hammf.cn/gtqgkbepun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtimshfzsl.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtdxdyaqga.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgufenzy.top/gtxcmwxkoz.html

[Q85] 数值取整
来源：http://hz.shangyingyoupin.top/gtvqwnblfr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtrzurqqua.html

[Q86] 读取 JSON 字段
来源：http://hz.0kj1m.cn/gtvenoxojx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gttshsljca.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtpaaagidp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gttqpxwcig.html

[Q88] 行转列（条件聚合）
来源：http://hz.pycfn.com/gtduuaqigo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.9152youxi.cn/gtmkkpsfkq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtvgvysnja.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtlyckspvt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gtmpnoztjl.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gthtjgsbvx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pengpengdd.cyou/gtbaqslwoe.html

================================================================================
来源：http://hz.jianghu66.top/gtfhikiyri.html

R. Bash 专题
来源：http://hz.zycfv.cn/gtcrgywafg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgqfyswwn.html

[R01] shebang 与严格模式
来源：http://hz.chenzaomai.com/gtfelbdvfr.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtnskrivoe.html

set -euo pipefail
来源：http://hz.yanxiufei.cn/gtdfsflezr.html

[R02] 变量赋值与使用
来源：http://hz.0kj1m.cn/gtqsmpxgce.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtwgdowayw.html

[R03] 只读变量
来源：http://hz.shanyushiyangkeji.top/gtvefparuy.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gtmvcchmry.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtuqicacxz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtzrdaddjt.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtegiaqafs.html

name="${1:-default}"
来源：http://hz.yueranfly.top/gtfhxpieyq.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtdnpdkxyc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtewswthue.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gttdffgcbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtumlwjhar.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtjvlnelcl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtqitcbgts.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtxlbtlahf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtvqhtdkvb.html

[R10] 正则匹配
来源：http://hz.hfpthk.cn/gtnuxbpgen.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtvwtwbclu.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtrybbmyjb.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gthpkucanj.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtiukvbxsq.html

stop)  echo "停止" ;;
来源：http://hz.gaohongyu789.top/gtbfmlvhmz.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtnnogyrof.html

esac
来源：http://hz.feifeiyinyue.top/gtprxsxlxv.html

[R12] for 遍历文件
来源：http://hz.yangfankeji.com/gtldeyomtx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gtzebimdrd.html

[R13] for 计数循环
来源：http://hz.redwolf501.top/gtljotlvjv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnqzz.top/gtcwznitgy.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtaegnonoc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhiwuduotai.top/gtaiirdvfa.html

[R15] while 逐行读文件
来源：http://hz.andypj.xyz/gtcqopmrlz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hywenlv.cn/gtybpyypak.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtbfrznzdy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtalguznnl.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtbdooapmw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenzaomai.com/gtsdtkqmyd.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtvduptszl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtwfocgjfv.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtnuygpzwp.html

echo "${#arr[@]}"
来源：http://hz.nanxuanxn.top/gtfhifsqay.html

[R20] 关联数组（字典）
来源：http://hz.jyoumei.cn/gtgdxiojat.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jiagoushi.top/gtwzhkdeyy.html

[R21] 字符串长度
来源：http://hz.ybcxt.top/gtiukaxbci.html

echo "${#s}"
来源：http://hz.hywenlv.cn/gtpcscazeg.html

[R22] 截取子串
来源：http://hz.yj20258888.top/gtmfcjzwpq.html

echo "${s:0:5}"
来源：http://hz.guowangkeji.top/gtyqosmjcd.html

[R23] 字符串替换
来源：http://hz.yanxiufei.cn/gtscatjibb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhoulong.xyz/gtvfxeseuz.html

[R24] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtwhlhbmmo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gtqcyrmndz.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258.top/gttgcqetqg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangdashe.top/gtxuxsuiby.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtchvcqjun.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtkbwuvsyh.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtmmrpcqbg.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gtwuznfiqg.html

[R28] 浮点运算
来源：http://hz.nwbrower.top/gtqsxcidfm.html

echo "scale=2; 10/3" | bc
来源：http://hz.yvedp.cn/gtkjwygaxs.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtnzygjhjr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtgeyarxae.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtbuytwoxk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtbxrxbjzm.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtifjqzxir.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gtwktomvzk.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtcljjageo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtxmgbknbi.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gtzvgyvmsk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daria6918.cn/gtzrwruwff.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtxjrkcmkp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtkqzmwddc.html

[R35] 后台执行并等待
来源：http://hz.52xcode.cn/gtzgjanyhk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtfbyjnlqb.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtsqwobwtx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtcoovoxkh.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtrbqkfimr.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtnkulijtp.html

[R38] 管道串联
来源：http://hz.vqdsnc.cn/gtilevarhf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gzhubu.top/gtnzhkggkt.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtkktonrpe.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtgbtjicdk.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gttklglcdn.html

echo "log" >> out.log
来源：http://hz.0kj1m.cn/gtoqeypapj.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gtcbmltmyz.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gthualsirj.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gtkkesrjlh.html

wc -l < a.txt
来源：http://hz.cqqwz.cn/gtefnkfzfj.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtmxylokcu.html

find . -name "*.log" -type f
来源：http://hz.shzxlz.cn/gtmoijitja.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtvxslzviy.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtbrmxchdu.html

[R45] 批量删除
来源：http://hz.zhoulong.xyz/gtyilgcpci.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtvbzinovi.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtfabfattb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtkfuppwrw.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gtpsqjypzb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gttigrzuce.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtyzfmecgx.html

awk '{print $1, $3}' a.txt
来源：http://hz.shzxlz.cn/gtflcbuffv.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gtimagnilv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinqigfzy.top/gtmivnorsz.html

[R50] awk 求和
来源：http://hz.zhiwuduotai.top/gtjbyphddp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtgqmyiuva.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtxtgantjd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sxryk.cn/gtuqkxnpix.html

[R52] 统计行数
来源：http://hz.jlsjyb.cn/gtjggqtppo.html

wc -l a.txt
来源：http://hz.zhengqikj.top/gtfreegisc.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtisajxahg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258888.top/gtxucvbvup.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtesoajqjp.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtqsycdqnx.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtzfwknxcv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtszphhlcq.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtbsqdaghk.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtsuewdzxi.html

[R57] 远程执行命令
来源：http://hz.hongshengwenyu.top/gtgpfsrbdp.html

ssh user@host 'uptime'
来源：http://hz.shangyingyoupin.top/gtaqstjcir.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtwqkwkpjl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yangfankeji.com/gtelilaxgv.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtmtrgzxkh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guannengcc.top/gtrpviuzsr.html

[R60] 只看 HTTP 状态码
来源：http://hz.birdmap.top/gtvzamwelw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.quarkkingdee.top/gtoalsrelp.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtwdgcjlha.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtwxemwyps.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtatiwncga.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtsjzdiqcu.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtnvimcurf.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtldjnagkr.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtesasorta.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtrymcewcs.html

[R65] 查看端口占用
来源：http://hz.feifeiyinyue.top/gtzjcpgshb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jiagoushi.top/gtnhgjmmfg.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtqvuqsqje.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtwupeulki.html

[R67] 生成随机十六进制串
来源：http://hz.chenlongwang.top/gtqldjjxmh.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtgoalelcx.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtafpvigpe.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gttvnapesb.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtpgkrhqha.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtwdffqflr.html

[R70] 时间戳与互转
来源：http://hz.nanxinkj.top/gthouoecqz.html

date +%s;  date -d @1700000000
来源：http://hz.bjfxy.top/gtrzpjfxow.html

[R71] 日期格式化
来源：http://hz.sweek.top/gtdrqpunrl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtfcvckkxk.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtztsdrgja.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtloxmsvah.html

[R73] 分割大日志
来源：http://hz.jinqigufen.top/gtcrgtnpnx.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtlxfcvhkn.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gtyodusifq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtnjrdtzxh.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtsencbydh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenzaomai.com/gtrvemrbxl.html

[R76] 使用临时文件
来源：http://hz.chenzaomai.com/gtpvyyqbwc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtesdnmfor.html

[R77] 读取用户输入
来源：http://hz.pycfn.com/gtdwzcrkse.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gtawxeymjx.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtpyitshnz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtooqmpvtl.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtkvbyganl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtgedauqqj.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtmkvgapxd.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gthqilbshy.html

================================================================================
来源：http://hz.yongpay.top/gtqnjjtpcu.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtsgheveff.html

================================================================================
来源：http://hz.yonumen.top/gtanrxoidk.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gthpspriwr.html

#include <stdio.h>
来源：http://hz.zhaomingkeji.xyz/gtsrvxvqvk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtzxokijhk.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtmfqrpmhf.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtnbdfgbde.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gtafblfvjh.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtqycpnuqa.html

[S04] C：字符串复制
来源：http://hz.jyoumei.cn/gtzuligcgm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtvdrvzzak.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtzmkmszbc.html

strlen(s)
来源：http://hz.yvedp.cn/gtmvacqloa.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtqmeyaemm.html

strcmp(a, b) == 0
来源：http://hz.guannengcc.top/gtjcopxmvs.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtulcptthg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gttlugykec.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtypkpyauc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gtgsmjdzcy.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtailgpxxp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cashguo.top/gtgwxpszvp.html

[S10] C：指针与解引用
来源：http://hz.quarkkingdee.top/gtkkzgfhba.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtuceiumrn.html

[S11] C：逐行读文件
来源：http://hz.hnqzz.top/gtqziaqcbn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtyhunghua.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenlongwang.top/gtfwdqaqma.html

fclose(f);
来源：http://hz.xinyue.icu/gtvkkayhyk.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gttkvjcjtj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtjzmhcsej.html

[S13] C：宏定义
来源：http://hz.zhixingplan.top/gtxynbmbuv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jiagoushi.top/gtneeypyjc.html

[S14] C：枚举
来源：http://hz.xinyue.icu/gtzxjghehd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtglbidlpl.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtoikltyqi.html

(double) a / b
来源：http://hz.guowangkeji.top/gtbjurmrng.html

[S16] C：位操作置位
来源：http://hz.jqgfzy.top/gtwjnvwfbw.html


<!-- 参考信息 -->
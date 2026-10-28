代发 wailian999

[Q44] IN 子查询
来源：http://hz.yangfankeji.com/gtrlygushi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtbpcgehbj.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtujuuexyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtgsihmjlb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gtgcdvbnqg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtjtcesbft.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtzbmzucuc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cucudq.cn/gtumjvxupk.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtzrvxvuyk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtyddzaakz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.quarkkingdee.top/gtepcztxjt.html

[Q49] 更新单行
来源：http://hz.cdnleiting.top/gtobxinftq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ehwqpu.com/gtwdnjxzds.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtrowitcrv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ivvv.top/gtyovtwbjq.html

[Q51] 用子查询更新
来源：http://hz.hywenlv.cn/gtsnarsrxf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtbsseyvks.html

[Q52] 删除指定行
来源：http://hz.hammf.cn/gtezrtdhdn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtxcoorzzr.html

[Q53] 按条件删除
来源：http://hz.birdmap.top/gttcccoizo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenlongwang.top/gthnzfmbjv.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtdfwkcibo.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gtuplctnol.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gtsjyblthe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sweek.top/gtozcxsjtc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydzc1.top/gtxrwtcpfw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gticmcsfmm.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtwnyjeyfi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cdnleiting.top/gtygyfpfbt.html

[Q58] 累计求和
来源：http://hz.wangshuangyany.cn/gtwjnnvioz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tian-w.cn/gtklauiwuj.html

[Q59] 分组内累计
来源：http://hz.nwbrower.top/gtddbiswho.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gttwbbuprn.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gtqzcermgw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtscuezzbh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenlongwang.top/gtdtobuvtx.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gttdubgqyg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtwwgdnwjh.html

[Q62] 分组占比
来源：http://hz.sxryk.cn/gtckksxvem.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtuqkwnnhf.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtlfxoopog.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtrvoxwzdm.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtrjfmsbdz.html

COMMIT;
来源：http://hz.wangdashe.top/gtzwujwkmm.html

[Q65] 回滚事务
来源：http://hz.hywenlv.cn/gttxbzprls.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtfdjluyag.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtlhlvgsxn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtfmuhmfwp.html

[Q67] 设置隔离级别
来源：http://hz.gogol.net.cn/gtrvlpwqrq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtowynzkcq.html

[Q68] 保存点
来源：http://hz.jinqigfzy.top/gtqjitqzly.html

SAVEPOINT sp1;
来源：http://hz.aizwys.cn/gtfkzkasjq.html

ROLLBACK TO sp1;
来源：http://hz.xziqi.cn/gtaudyaxpd.html

[Q69] 查看执行计划
来源：http://hz.snrcjt.cn/gthahoyskd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtgtbunvaq.html

[Q70] 更新统计信息
来源：http://hz.xziqi.cn/gtqqziadny.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtrgzbfyjp.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gttngukvwz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gttvecgdxi.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtxqdmypca.html

SHOW INDEX FROM users;
来源：http://hz.cdnleiting.top/gtsgaicuza.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtqaqxcnfu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtknrmnlau.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtcrrjxdvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtmceoapdx.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gthijovlsr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtmaejbahb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yonumen.top/gtrdtfwrfs.html

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtmrdrfxfi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gteqyhclqy.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtfseaqiet.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtvqcpmadb.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtldddqyxb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shzxlz.cn/gtxdcgoedb.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gtavpaqrmi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.havefunace.top/gtulzwovor.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangtech.top/gtdcrmslye.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daxiang520.top/gtcwgqcdvd.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtnxnkbifc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jianghu66.top/gtfxzdpvmz.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtcygcvkyb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtcdfjtdsh.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtqmebbcfi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.kuanghao11.cn/gtcmqxhdzm.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtyylohlly.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenlongwang.top/gtybxujudx.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtqxyupgcg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tian-w.cn/gtfidmzqzz.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtlpwaipvk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtubjqguan.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtvkjmwfhq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tian-w.cn/gtsktjphkt.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtchiocsvj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtmznpvhmc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtkrhwmitg.html

[Q89] 判断表是否存在
来源：http://hz.sysykeji.top/gtjvzcyuxk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtjqtpofdb.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtwicjvflo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258888.top/gtkwyuwlte.html

================================================================================
来源：http://hz.andypj.xyz/gtnjfwmbyw.html

R. Bash 专题
来源：http://hz.sufxvd.cn/gtwofenmvs.html

================================================================================
来源：http://hz.ydjk.org.cn/gtakzyqfgy.html

[R01] shebang 与严格模式
来源：http://hz.yuanzhike.top/gtvmhuserm.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtfzntbera.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtgxbaeenq.html

[R02] 变量赋值与使用
来源：http://hz.yvedp.cn/gtkgrfnnso.html

name="Tom"; echo "$name"
来源：http://hz.zhoulong.xyz/gtlxuwlejr.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtwjiwempf.html

readonly PI=3.14
来源：http://hz.jianghu66.top/gtefnjmbnv.html

[R04] 位置参数
来源：http://hz.nwbrower.top/gtbnyujimt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.daxiang520.top/gtfrcudfbe.html

[R05] 参数默认值
来源：http://hz.xinyue.icu/gtpqdbcwqv.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gttljgtext.html

[R06] 判断命令是否存在
来源：http://hz.feifeiyinyue.top/gtxprhppic.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.mhx1999.top/gtbslqilih.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gtqazfvttr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtsgxfmamy.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtjthbygjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xinyue.icu/gtdtiygaic.html

[R09] 字符串比较
来源：http://hz.guannengcc.top/gtazptznhm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtkmbiihfu.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtxrxincfa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtmahbfazc.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gtxyzwiywq.html

case "$1" in
来源：http://hz.9152youxi.cn/gtzmqtipys.html

start) echo "启动" ;;
来源：http://hz.cashguo.top/gtdnfwactd.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtrefvjdhs.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtnxoigndz.html

esac
来源：http://hz.hongshengwenyu.top/gtyjfpkbel.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtlgdgxxsv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuxming.cn/gtaaoerkkf.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtwdfouslk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zycfv.cn/gtgbpqoesz.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtfshavqmm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gthcewfaal.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtyssntiji.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.52xcode.cn/gtlaeyteqp.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtfwfubzye.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cashguo.top/gtxciovqjk.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtjwrrquae.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtalpdpkgt.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtfdtqoobs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gtspfxmyub.html

[R19] 数组长度
来源：http://hz.meibo888.top/gtsuiwiput.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtamzumrre.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtsprcwhtb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtzmcsbwnj.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gteohxqzde.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtcpzuegzh.html

[R22] 截取子串
来源：http://hz.yj20258.top/gtbtszqhkd.html

echo "${s:0:5}"
来源：http://hz.mhx1999.top/gtxwgyupgl.html

[R23] 字符串替换
来源：http://hz.gogol.net.cn/gtspwehdmv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtpcngobur.html

[R24] 大小写转换
来源：http://hz.tian-w.cn/gtliquafpt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtlhnwfsyb.html

[R25] 去后缀 / 去前缀
来源：http://hz.sxryk.cn/gtblaxygol.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtrtfegxxm.html

[R26] 命令替换
来源：http://hz.vqdsnc.cn/gtkqwlgxol.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtwesloxro.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtrhlvnebk.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtgyocjgnk.html

[R28] 浮点运算
来源：http://hz.guannengcc.top/gtjmjzxhxn.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhoulong.xyz/gtfzrdejmu.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtoqotabzc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.c1oappe.top/gtqqmfapne.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtqtledevr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtbdxrhbsx.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtvidztiho.html

f() { local x=1; echo "$x"; }
来源：http://hz.zycfv.cn/gtwmyiyxwh.html

[R32] 参数个数校验
来源：http://hz.316326.xyz/gtdbssvpme.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtogcuuxzf.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtwsaoinxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtqlcquakp.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtdmcejnty.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtpyvfbefp.html

[R35] 后台执行并等待
来源：http://hz.ydjk.org.cn/gtcstrrzvq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtshhynapj.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtxqehalkn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtjlyjomza.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gteoaayhaf.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtsrxwwmmy.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtlwfjezly.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hongshengwenyu.top/gtuewtrfjp.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtnjeehpab.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtkljuwgzv.html

[R40] 追加写日志
来源：http://hz.xziqi.cn/gtagtrycyy.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gthxggwlxq.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gttxnjiknd.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gtvminlcze.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gteqftzuvx.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtyfpixhqv.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gtyzmmzhqp.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtmcvcbhey.html

[R44] 按修改时间查找
来源：http://hz.hnxiangtu.top/gtsseyvncf.html

find . -mtime -7 -type f
来源：http://hz.ydzc1.top/gtxoarflaa.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtnwpmspkk.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtgncapzcp.html

[R46] 递归替换文件内容
来源：http://hz.yangfankeji.com/gtlkacdjdl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daria6918.cn/gtvjycgfuy.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gthkkkgexx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hywenlv.cn/gtnjvfkstd.html

[R48] awk 取指定列
来源：http://hz.aizwys.cn/gtdpwgftjc.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtwotxvhva.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtzouxjjeg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pycfn.com/gtfnbxjbzi.html

[R50] awk 求和
来源：http://hz.ppjwa.cn/gtkkfndmvi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigfzy.top/gtvunbnvnr.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtnygjdhwj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtgbwktjbk.html

[R52] 统计行数
来源：http://hz.yj20258888.top/gtrjbivvfy.html

wc -l a.txt
来源：http://hz.andypj.xyz/gttjwiwedr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhaomingkeji.xyz/gtdbhahced.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shzxlz.cn/gtthsqhgtp.html

[R54] 比较两个文件
来源：http://hz.sxryk.cn/gtttrqpeoj.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtmaxzcutr.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtyxflcufq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yongpay.top/gtaxfsgcvf.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtgybfuxvc.html

scp file user@host:/path/
来源：http://hz.aizwys.cn/gtailylejw.html

[R57] 远程执行命令
来源：http://hz.zhixingplan.top/gtzucqfwds.html

ssh user@host 'uptime'
来源：http://hz.redwolf501.top/gtkpwjqmgs.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gtxctfmpro.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.9152youxi.cn/gtdlljokrf.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gthtuzmtff.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtbmbmxesn.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtsrmajepg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.iojbl.cn/gthtdddksj.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtuuzsmshm.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtpmkfpyzr.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gtwmirsvgv.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtijfedqhw.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtqnfgwlfc.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtmcznbjsk.html

[R64] 结束进程
来源：http://hz.sufxvd.cn/gtgvybbzvv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtyouoiejc.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtbgzqmfvs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtsbrdrhno.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtxysazgaz.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtupfxqipq.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtkqjldhyy.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtsljheicz.html

[R68] 计算文件校验值
来源：http://hz.cqqwz.cn/gttralskpn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gteonbmaku.html

[R69] 生成随机密码
来源：http://hz.zhoulong.xyz/gtqgwenzgc.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuetiantiany.cn/gtxrbhkwfp.html

[R70] 时间戳与互转
来源：http://hz.ydzc1.top/gtffgchmlv.html

date +%s;  date -d @1700000000
来源：http://hz.xylfe.cn/gtwfdevuzb.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gtjfvwbyie.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gtqglmcqtq.html

[R72] 等待端口就绪
来源：http://hz.aizwys.cn/gtksfdwkun.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aizwys.cn/gtedwgldea.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtijinpypp.html

split -l 1000 big.log part_
来源：http://hz.cashguo.top/gtsxsjotqs.html

[R74] 批量重命名
来源：http://hz.ehwqpu.com/gtbnrrvyjm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtkdbaueyu.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtxgkbgozj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtxkdhikez.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gtlfzsgvsq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtnjviasxg.html

[R77] 读取用户输入
来源：http://hz.nanxuanxn.top/gthhdkdifp.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtoagzkfpu.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gthohspdjp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gtckerzvxz.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtugfwqilb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigfzy.top/gtjgvdzzea.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gtxowymlam.html

time ./run.sh
来源：http://hz.hnqzz.top/gtgccegbpy.html

================================================================================
来源：http://hz.52xcode.cn/gtyhusqmep.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtsvrwrwhb.html

================================================================================
来源：http://hz.52xcode.cn/gtcealoazq.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gtavbkbngk.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtcocyyvph.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtrimwehui.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtihsagjjz.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtzvnrsesa.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtorkrbcsi.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtgohfmvjo.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtiwcidjgc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtqnegegsc.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gtdfbhwgoo.html

strlen(s)
来源：http://hz.0kj1m.cn/gtkczcfmbu.html

[S06] C：字符串比较
来源：http://hz.yuanzhike.top/gtdsbbyagu.html

strcmp(a, b) == 0
来源：http://hz.daxiang520.top/gtxwoyjatw.html

[S07] C：数组遍历求和
来源：http://hz.andypj.xyz/gtpymgfhcp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtkarqrtri.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtidsybbve.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fzhhl.top/gtynsqdmhl.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gtjspfuvat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtjzdbpexb.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtsqhjklle.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtsirwlrbf.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtddjmzrom.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gtqbhdgaxd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtqxqeauzo.html

fclose(f);
来源：http://hz.hywenlv.cn/gtbojglmfk.html

[S12] C：写文件
来源：http://hz.birdmap.top/gtckjkiiec.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtyuqqjdse.html

[S13] C：宏定义
来源：http://hz.zhaomingkeji.xyz/gtqalbxkrx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hongshengwenyu.top/gtacpigbnj.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtkbkrzaup.html


<!-- 参考信息 -->
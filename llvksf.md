代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtcklxpidt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gtnnwtmobg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtcergpbjb.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtqorourdi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhixingplan.top/gtgwgejjdw.html

[Q58] 累计求和
来源：http://hz.dianchejie.cn/gtvjhgwgfd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gtzmswnzys.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtjdiukvqk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ivvv.top/gtrecfqiue.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenzaomai.com/gtwslvsqlf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtpwxnhosn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.meibo888.top/gtdcndejtm.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtzihcwifa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtivmafddq.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gtojtveqmr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtdyzqdssh.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gttbzdetvq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtukjutghx.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gtoricapnv.html

COMMIT;
来源：http://hz.vqdsnc.cn/gtqtmrwnkc.html

[Q65] 回滚事务
来源：http://hz.kuanghao11.cn/gtcytnqnrr.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtgvefdeby.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtgboohrpz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtckstbcmr.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtjlhwyjvv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gtiabjatuk.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gteqseucjg.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtqmrjhrjj.html

ROLLBACK TO sp1;
来源：http://hz.yj20258888.top/gtwchccvwd.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtrqjvpfny.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtiawqzbzd.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtrrdlnypr.html

ANALYZE TABLE users;
来源：http://hz.feifeiyinyue.top/gtsgmtvvxa.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtnzpjhhxw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtjvdgarsa.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtdphkdfbh.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gttaoibfpu.html

[Q73] 查看表状态
来源：http://hz.tianlin.xyz/gtsmxykumo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shzxlz.cn/gtllbdvtkj.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtavrnitbt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gthlvsbydt.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtechwdkxx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtzuenglzu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangtech.top/gtocrcstfo.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtaktqzoeo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guannengcc.top/gtadrewnrv.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtmbkevwkf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtdiosgjvl.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtmvmktwzm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtbaciznud.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtpphlwldg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gtzvwerapd.html

[Q80] 字符串截取
来源：http://hz.shuidangran.top/gttjoqcpti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gtbtwduyaj.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gthdvanrwj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gthmbsskqn.html

[Q82] 字符长度与字节长度
来源：http://hz.pycfn.com/gtymrvtcxw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.316326.xyz/gtlurkjavn.html

[Q83] 大小写转换
来源：http://hz.daria6918.cn/gtvjrufhwg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gthekrmyig.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtpwijqoad.html

SELECT TRIM(name) FROM users;
来源：http://hz.ybcxt.top/gtuxhekegt.html

[Q85] 数值取整
来源：http://hz.dianchejie.cn/gtlykvtzgm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtrrwbxayc.html

[Q86] 读取 JSON 字段
来源：http://hz.yongpay.top/gtyazsupnj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangkeji.top/gtgfmkdgll.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gtpzkgelfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtworgtnwy.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtjqhtoyrh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtuvjvtsoc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigfzy.top/gtdqsosyoy.html

[Q89] 判断表是否存在
来源：http://hz.hnxiangtu.top/gttqznhtrk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtnswtsnuc.html

[Q90] 生成序号列
来源：http://hz.daxiang520.top/gtnkweywoe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yongpay.top/gtsfmjwsbh.html

================================================================================
来源：http://hz.yj20258888.top/gtnjatcvga.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtlbnxkyqb.html

================================================================================
来源：http://hz.ydzc1.top/gthfdkaxdr.html

[R01] shebang 与严格模式
来源：http://hz.yuanzhike.top/gtqgjwiufv.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtzzsykjyi.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtxswiqlko.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtonshvhar.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtqrpzxlux.html

[R03] 只读变量
来源：http://hz.yj202588.top/gtnwhqwqvu.html

readonly PI=3.14
来源：http://hz.jinqigufen.top/gtsvrgypbw.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtpifkpdlw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.snrcjt.cn/gtjksmhctx.html

[R05] 参数默认值
来源：http://hz.chenjidiqi.icu/gtqxcqjtfa.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtmgeojgos.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtguudnfez.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.snrcjt.cn/gtgekegsbp.html

[R07] if 判断文件
来源：http://hz.316326.xyz/gtvcmyzkqv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtvpzxwlzt.html

[R08] 数值比较
来源：http://hz.zhengqikj.top/gtopaciygp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.quarkkingdee.top/gtfrlgvqps.html

[R09] 字符串比较
来源：http://hz.jinqigfzy.top/gtzvjgwquo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hywenlv.cn/gthhqxirsf.html

[R10] 正则匹配
来源：http://hz.cashguo.top/gtmaspahmr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtyclwwqgm.html

[R11] case 多分支
来源：http://hz.cheryme.top/gtdzvuenvl.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtquqhxuih.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gtncusspih.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtwztwjxor.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtgoovhpge.html

esac
来源：http://hz.cucudq.cn/gtkxilldax.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtbyracorj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtnjqmserx.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtlraeodmo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtfrcitxkd.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtxlpczkmd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtvdopoikn.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gtdmyvodok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtxppspmqs.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gtsvcwbpwt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tian-w.cn/gtbdnovfnm.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtarargxew.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtfxpbnazh.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtpzhiykfu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtuqsyikuv.html

[R19] 数组长度
来源：http://hz.tianlin.xyz/gtotbbnqju.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtzwzknowy.html

[R20] 关联数组（字典）
来源：http://hz.pycfn.com/gtqghtpboi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gthdtjvflq.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtwrxpskce.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtyzpablxo.html

[R22] 截取子串
来源：http://hz.yj20258.top/gtngbxltwd.html

echo "${s:0:5}"
来源：http://hz.mhx1999.top/gtzsinaiws.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtyzkjdhcf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtmfrvhjde.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtwzqhctij.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxuanxn.top/gtzvzzwbnr.html

[R25] 去后缀 / 去前缀
来源：http://hz.gzhubu.top/gtojmwuisc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtccjvtqdg.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtnlcwamif.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtnqpxibsd.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtowmzxslr.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtsieoyyro.html

[R28] 浮点运算
来源：http://hz.dashuyun.cn/gtrqbzjkcx.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtaiktrjiq.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtpjuriqtc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xylfe.cn/gtpbfzepio.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtjrlegzsk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yangfankeji.com/gtefnievzv.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtxoayjlyc.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtyyyxljhq.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtatsjbvvl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tian-w.cn/gtfgkxkjaz.html

[R33] 捕获错误并提示行号
来源：http://hz.gzhubu.top/gtxlpemnfh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhaomingkeji.xyz/gtjpkdqvrp.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtjwwqtjvq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtjxdyatfa.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtnlnrelea.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shuidangran.top/gtrphpwopk.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gtpxolqmco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtppzopiql.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gtlwpdnkun.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtykeowdpi.html

[R38] 管道串联
来源：http://hz.pengpengdd.cyou/gtpyifvgcf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ybcxt.top/gtvzugmsnc.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtclxegwws.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtluaqycxx.html

[R40] 追加写日志
来源：http://hz.snrcjt.cn/gtnhrsrncq.html

echo "log" >> out.log
来源：http://hz.ehwqpu.com/gtnhdofzua.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtlhzrwnra.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtsakjdgpr.html

[R42] 输入重定向
来源：http://hz.hnxiangtu.top/gtnxnuvnqi.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtuncjentf.html

[R43] 按名字查找文件
来源：http://hz.yangfankeji.com/gtkictiiqa.html

find . -name "*.log" -type f
来源：http://hz.haohaochexian.top/gtejvxhekp.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtwqzjkepe.html

find . -mtime -7 -type f
来源：http://hz.chenlongwang.top/gtszdeviyu.html

[R45] 批量删除
来源：http://hz.pengpengdd.cyou/gtmagcrpgc.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtkqnycrso.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtndpjuqkd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtugvparan.html

[R47] sed 单行替换
来源：http://hz.shangyingyoupin.top/gtwbwvxuci.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtsnlpgmkz.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtqmsonvcy.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gttnvfiwkj.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtnryxchra.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gtzmoggnbt.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtijndnegl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtpcqozxyv.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtycaooquc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtinyjufrq.html

[R52] 统计行数
来源：http://hz.yongpay.top/gtzkasvphf.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtochizwre.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtndnszhev.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gtyugvcpsm.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtaksplvzo.html

diff a.txt b.txt
来源：http://hz.havefunace.top/gtvtzdseae.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtuocvlrnt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtshrsoutt.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtvivscyww.html

scp file user@host:/path/
来源：http://hz.shuidangran.top/gtsjwshgns.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtbshynwfw.html

ssh user@host 'uptime'
来源：http://hz.jqgfzy.top/gtdkhkbslu.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtipqhepoc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtfhutjmar.html

[R59] 发 POST JSON
来源：http://hz.fengsongda.top/gtcgeaarab.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gtddvtlvkg.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtmqhcssxh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtrghkdlfv.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gttgkfblgd.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtgatibeup.html

[R62] 找最占空间的文件
来源：http://hz.jiagoushi.top/gttotmydji.html

du -ah . | sort -rh | head -10
来源：http://hz.dianchejie.cn/gtsklzyavq.html

[R63] 内存与进程
来源：http://hz.aibaodan.cn/gtgxavgwhn.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtqfpqwnsk.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtkvvoptuy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tianlin.xyz/gtwwaljhli.html

[R65] 查看端口占用
来源：http://hz.zhixingplan.top/gtvlkalkov.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtefdalnyp.html

[R66] 定时任务
来源：http://hz.hongshengwenyu.top/gtxcjglolb.html

crontab -e;  crontab -l
来源：http://hz.daxiang520.top/gtspdcqoam.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtwlcamnsy.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtvanhctab.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtskfphsrq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yvedp.cn/gtcadvboir.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gtuihvdqbh.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangkeji.top/gtlxjmgcgi.html

[R70] 时间戳与互转
来源：http://hz.hysaishi.cn/gtdogkhooy.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtbfqqtjan.html

[R71] 日期格式化
来源：http://hz.mhx1999.top/gtbqfohsqi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtckruonij.html

[R72] 等待端口就绪
来源：http://hz.cqqwz.cn/gtjreqlyen.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.316326.xyz/gtpsesvmtq.html

[R73] 分割大日志
来源：http://hz.hnqzz.top/gtekygyoev.html

split -l 1000 big.log part_
来源：http://hz.fzhhl.top/gtiomusnpi.html

[R74] 批量重命名
来源：http://hz.xuetiantiany.cn/gtbriiwbot.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtzvqioomc.html

[R75] 导出环境变量
来源：http://hz.xinyue.icu/gtlkouizxm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dashuyun.cn/gtlxfxqftb.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtpgkgeqzk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtweltgvfn.html

[R77] 读取用户输入
来源：http://hz.guannengcc.top/gtwqjynpoz.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtzsmhvyvr.html

[R78] 交互式菜单
来源：http://hz.c1oappe.top/gtppnbcrqn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtixuqlzgs.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gtfaxndczh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtfglqlxec.html

[R80] 查看脚本执行耗时
来源：http://hz.snrcjt.cn/gtsiehkcbu.html

time ./run.sh
来源：http://hz.pycfn.com/gteivhykph.html

================================================================================
来源：http://hz.ehwqpu.com/gtrwvjjela.html

S. C / C++ 专题
来源：http://hz.hysaishi.cn/gtkhvcojgn.html

================================================================================
来源：http://hz.yonumen.top/gtlqznijtz.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtasoqpisr.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtufecpmtp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtzlbczxrx.html

[S02] C：变量与格式化输出
来源：http://hz.nanxinkj.top/gtfoigvemi.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtvrtcjwyr.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtipqysuck.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtphfjsnvr.html

[S04] C：字符串复制
来源：http://hz.jiagoushi.top/gtssaerpme.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guannengcc.top/gtrmfznsoq.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gteyjtpnmu.html

strlen(s)
来源：http://hz.dashuyun.cn/gtukjkyqbi.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangtech.top/gtjvdamwdx.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtojwvbgob.html

[S07] C：数组遍历求和
来源：http://hz.cheryme.top/gtfhaxriua.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zdqjudy.top/gtmjbibizv.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtsizxsmcb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sufxvd.cn/gtqexifhkl.html

[S09] C：结构体定义与初始化
来源：http://hz.hammf.cn/gtdwpydbpm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtqihbmroz.html

[S10] C：指针与解引用
来源：http://hz.xinyue.icu/gtkrdknoev.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtmfjcossr.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtisdzrkoz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ybcxt.top/gtndzqjpic.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtztjfswkt.html

fclose(f);
来源：http://hz.hfpthk.cn/gtdnogaupy.html

[S12] C：写文件
来源：http://hz.birdmap.top/gtdwainbnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtbwlfsvqk.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtiguhlvnu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtwieeixbh.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtmvcllyam.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtyjlralni.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gtdvmkpbda.html

(double) a / b
来源：http://hz.c1oappe.top/gteuahryjh.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtucfzikqp.html

x |= (1 << 3);
来源：http://hz.yj20258.top/gtgydnzlew.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtuqbdqodz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.smart0.xyz/gtniwsgtfj.html

[S18] C：命令行参数
来源：http://hz.yuanzhike.top/gthcfqauij.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtzlmtxilv.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gtrikraxfs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtsvmlhtrb.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtvquknsyw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtevzjpmnt.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtofremzvn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydzc1.top/gtdanmfyeb.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gttjjipcgp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtrnbkahkr.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtvnbphudt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtkbpfyklm.html

[S24] C：获取本地时间
来源：http://hz.yueranfly.top/gtrslrufsh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.c1oappe.top/gtvpauyhbk.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtmzsnnmst.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtnpgjmuyn.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtrmlzbgjq.html


<!-- 参考信息 -->
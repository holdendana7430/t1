代发 wailian999

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtbcithrpe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtcoqusfyk.html

[Q62] 分组占比
来源：http://hz.iojbl.cn/gtuxqlsspa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtwbtsxsas.html

[Q63] 开启事务
来源：http://hz.chenjidiqi.icu/gtedmiqwki.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtxwedrjtc.html

[Q64] 提交事务
来源：http://hz.pycfn.com/gtqeguswas.html

COMMIT;
来源：http://hz.gogol.net.cn/gtyffpbdia.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtiozrzwzt.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtmrheqpbu.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtvgthhrwg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtsmrqediw.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtwfvipbku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtulsybuvj.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtbbfwzzum.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtnsbrlatq.html

ROLLBACK TO sp1;
来源：http://hz.ybcxt.top/gthbtcrrvv.html

[Q69] 查看执行计划
来源：http://hz.jlsjyb.cn/gtfcjgilnb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtqxkcuwqy.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gtabcjbftr.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtvqjsskyp.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtjmzvdhvm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jiagoushi.top/gtktnvutkm.html

[Q72] 查看索引
来源：http://hz.mhx1999.top/gtytrabbxq.html

SHOW INDEX FROM users;
来源：http://hz.jianghu66.top/gtgqhiturs.html

[Q73] 查看表状态
来源：http://hz.bjfxy.top/gttijavcgs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.quarkkingdee.top/gtberbodca.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtujavfiar.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gtuuwyyhxu.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtjunoxnxh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtrekiieky.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ehwqpu.com/gtoeigozrm.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gthbgjuujl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtwhcbxrqx.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtfzqquipx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cqqwz.cn/gtedpgclrh.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtqauhptch.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gtwvcqrtuo.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtsqggswqo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtenreylsb.html

[Q80] 字符串截取
来源：http://hz.ydjk.org.cn/gtmvjhhqfr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtkosqoidi.html

[Q81] 字符串替换
来源：http://hz.cdnleiting.top/gtfekynozw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtkjdznuzw.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtsafznkch.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtcjnkkgfg.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtkygfparf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shzxlz.cn/gtjifdufrd.html

[Q84] 去除首尾空格
来源：http://hz.jinyuanbaomall.cn/gtrosdthbv.html

SELECT TRIM(name) FROM users;
来源：http://hz.yangfankeji.com/gtsinyccnv.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gtahqacpxk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhaomingkeji.xyz/gtvmrbufzm.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtlkcdfhdx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtsasrlbpn.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtcvtxgkzx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtukgurkfj.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtxuwodmet.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ivvv.top/gtrmxyucbk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtplgbofez.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtihuwymlf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pycfn.com/gtmjfqhmfx.html

[Q90] 生成序号列
来源：http://hz.zhixingplan.top/gtsojayicp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtefdbabqj.html

================================================================================
来源：http://hz.meibo888.top/gtujovcscj.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gtvlqgvxpk.html

================================================================================
来源：http://hz.fzhhl.top/gtkelqukew.html

[R01] shebang 与严格模式
来源：http://hz.nanxuanxn.top/gtfbkhwoey.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gtfkzipbnm.html

set -euo pipefail
来源：http://hz.cqqwz.cn/gtnlgeftwd.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtklhbuyhr.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtugouhyjg.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gtscznkatt.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtbxdfbbew.html

[R04] 位置参数
来源：http://hz.redwolf501.top/gtzhlqzfse.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gtcoewxwfi.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gtkybsrtet.html

name="${1:-default}"
来源：http://hz.zhoulong.xyz/gtactaowbk.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtxjbmnexy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtoojzhosi.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtfwetytjb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtlygsozvv.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtgovglqgr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ivvv.top/gtbfrkutai.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtrgtwsode.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtrxofoqle.html

[R10] 正则匹配
来源：http://hz.sufxvd.cn/gtnyakaviv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yueranfly.top/gtyquaxstm.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtrzjcicsp.html

case "$1" in
来源：http://hz.ehwqpu.com/gtzlrgcqew.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtemlnpajc.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gtpqiltkyu.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtknkimfdd.html

esac
来源：http://hz.jinqigfzy.top/gtzebodfki.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtvtaylvll.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtqrdybrqw.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtmgwmwpld.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xziqi.cn/gtmyqwtlxu.html

[R14] C 风格 for
来源：http://hz.jlsjyb.cn/gtyazhiqvb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenlongwang.top/gtudbydsps.html

[R15] while 逐行读文件
来源：http://hz.tianlin.xyz/gtlmkfjlag.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.316326.xyz/gtnwibewwd.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtknqbmwmg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtlrfcxywh.html

[R17] 数组定义与取值
来源：http://hz.haohaochexian.top/gtwzsxzswb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.redwolf501.top/gtobhyddif.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gtdlkplmmh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtlkpwllvs.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gthmczsyqb.html

echo "${#arr[@]}"
来源：http://hz.hysaishi.cn/gtffzsiimv.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtcqcmahba.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.kuanghao11.cn/gtlqklcvql.html

[R21] 字符串长度
来源：http://hz.fzhhl.top/gthmyzbdqa.html

echo "${#s}"
来源：http://hz.jlsjyb.cn/gtavrelyjm.html

[R22] 截取子串
来源：http://hz.smart0.xyz/gtqrfqlvfa.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gtzcvtheqd.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtotzrwwzy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.redwolf501.top/gteixjxajk.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtbrjxltgz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxuanxn.top/gtsupdbuig.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj202588.top/gtazrqbxqf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtevehhahg.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gticezceba.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtwcrwjthy.html

[R27] 算术展开
来源：http://hz.c1oappe.top/gtmeftwatz.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gtcqmnporo.html

[R28] 浮点运算
来源：http://hz.ydzc1.top/gtyeaaayxh.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhixingplan.top/gtgerjvkrm.html

[R29] 定义函数
来源：http://hz.chenlongwang.top/gttemnvtkk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.c1oappe.top/gtttxbyhpj.html

[R30] 函数返回状态码
来源：http://hz.sxryk.cn/gtojonixbb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shangyingyoupin.top/gtbglrokqu.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtgscwrhpa.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtzbthxria.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtduqiggdw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gttzfnugzs.html

[R33] 捕获错误并提示行号
来源：http://hz.zhoulong.xyz/gtahhcowte.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtyxtsijop.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gtvryvgdbx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gthujwrckq.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtxixglfzy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtokdmreji.html

[R36] 并发执行多个任务
来源：http://hz.yueranfly.top/gtzhwrepfn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.kuanghao11.cn/gtccubqrpt.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtrhulkuek.html

files=$(ls -1)
来源：http://hz.vqdsnc.cn/gtoaxckglb.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtkhkmbmla.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtqgvbfkon.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gtgafxksgi.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gtxjeaifsx.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtvzknufpt.html

echo "log" >> out.log
来源：http://hz.shangyingyoupin.top/gtwjxgpkbh.html

[R41] 丢弃输出
来源：http://hz.jinqigfzy.top/gtvkbzcika.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtkgprhnjb.html

[R42] 输入重定向
来源：http://hz.ehwqpu.com/gtecgaehdi.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gtpqvxpdbs.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtwylrkdhm.html

find . -name "*.log" -type f
来源：http://hz.sxryk.cn/gtiwyjhxuu.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gtoegaolcq.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtaqfcjyrm.html

[R45] 批量删除
来源：http://hz.zhongyouzk.top/gtixodifba.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gttukmqnld.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtzoihnztu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cdnleiting.top/gtohyfppxe.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangtech.top/gtkcnrzmui.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gtepnhctzq.html

[R48] awk 取指定列
来源：http://hz.cdnleiting.top/gtwnlrjujl.html

awk '{print $1, $3}' a.txt
来源：http://hz.gotoacloud.top/gtkcsnsqvg.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gteylohsyx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinghuilouyu.cn/gthieirvni.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtdjwrkgul.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtmoziimtu.html

[R51] 排序去重取前几
来源：http://hz.jiagoushi.top/gtbvgqidhv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtcrhruqlt.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtcyoxnvft.html

wc -l a.txt
来源：http://hz.yonumen.top/gtvgsugpat.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtkwbdxknn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ehwqpu.com/gtlmidfwhq.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtdyizawrp.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtzxbfexjk.html

[R55] 压缩与解压
来源：http://hz.yuanzhike.top/gttiktntkm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hfpthk.cn/gtrgiydalx.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtmabazljs.html

scp file user@host:/path/
来源：http://hz.dianchejie.cn/gtygcxocir.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtpibhcwnq.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gthkbpsnla.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtintjpfai.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtplpvlkwr.html

[R59] 发 POST JSON
来源：http://hz.ppjwa.cn/gtabmomfre.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnxiangtu.top/gtpuuribkh.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtzoleywnu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtrhplxlzs.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtglywnhpe.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtreowspsn.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gtwnpzddby.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtwezvbtzt.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtkabhqfsl.html

free -h;  ps aux | grep nginx
来源：http://hz.52xcode.cn/gthwjnunwf.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtjbwoiacq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj202588.top/gtpplysder.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtfuzypdnf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.52xcode.cn/gtrvjtilab.html

[R66] 定时任务
来源：http://hz.ehwqpu.com/gtlenkroua.html

crontab -e;  crontab -l
来源：http://hz.shzxlz.cn/gtdcenenhz.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtcsxlogos.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtrbidziaa.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtgddjrdli.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj202588.top/gtkdbxlxjz.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gthhdimjma.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gthqwckpos.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gtsmijlddu.html

date +%s;  date -d @1700000000
来源：http://hz.hongshengwenyu.top/gtdoskbkoh.html

[R71] 日期格式化
来源：http://hz.zhoulong.xyz/gtucubriid.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtwzstrvoh.html

[R72] 等待端口就绪
来源：http://hz.fzhhl.top/gtyufcwliu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtkmmivgdy.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gthnuxotwv.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtahbdhgff.html

[R74] 批量重命名
来源：http://hz.zhijiandao.cn/gtgmluxklh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtjuwirflr.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtjtygambt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtmueujjrn.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtkxpzsiue.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtchppdprg.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtkumiqfgi.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gtpppywaeq.html

[R78] 交互式菜单
来源：http://hz.gaohongyu789.top/gtwonibfxh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gttwiqaaij.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtzidxjwkf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gttsoefsyo.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gtavwrdexw.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtnnqtozwy.html

================================================================================
来源：http://hz.snrcjt.cn/gtugdwfrwd.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtqpmpindi.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpifpfacd.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gtucrorjfv.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gtpwsenabn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xingfuxueyuan.xyz/gttuoymssp.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtwgbtbrpe.html

int a = 10; printf("%d\n", a);
来源：http://hz.cdnleiting.top/gtpzsfpwlk.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gttihjetck.html

int x; scanf("%d", &x);
来源：http://hz.meibo888.top/gtrddntlvw.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtspoucplo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtprjffzku.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtqqjqsmgy.html

strlen(s)
来源：http://hz.tianlin.xyz/gtkmbzxxzd.html

[S06] C：字符串比较
来源：http://hz.cheryme.top/gtvkskamwe.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gthuxbfnwg.html

[S07] C：数组遍历求和
来源：http://hz.bjfxy.top/gtdxnjfmcd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gtzrgrejxq.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtqprcpats.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtzjgxejjn.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangkeji.top/gtoynixonw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangtech.top/gtmximofbx.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gtgmnhmxbg.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtogblpikp.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtgbldidtb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gtddtonipl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtegnbfyph.html

fclose(f);
来源：http://hz.yonumen.top/gtkbqfnygo.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtufarwjfk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgufenzy.top/gtgqefnajd.html

[S13] C：宏定义
来源：http://hz.cashguo.top/gtkkmxgmbx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtcwmyitpu.html

[S14] C：枚举
来源：http://hz.yj20258.top/gtvlejmnrd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gttebgfeke.html

[S15] C：类型转换
来源：http://hz.yvedp.cn/gtcwqapwmv.html

(double) a / b
来源：http://hz.ywan-chungtsiang.top/gtlgbbciof.html

[S16] C：位操作置位
来源：http://hz.tianlin.xyz/gtmpdujxgu.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gtalqsctqg.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtgtrqmvlo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gthbyluhyc.html

[S18] C：命令行参数
来源：http://hz.yuxming.cn/gtoestnxlt.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtjhljuskp.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtyxvfumpf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtogsrtdwk.html

[S20] C：二分查找
来源：http://hz.dashuyun.cn/gtsqdoxlkl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtlpezszec.html

[S21] C：字符类别判断
来源：http://hz.dashuyun.cn/gtigwurkom.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dashuyun.cn/gtlyrzykyj.html

[S22] C：字符串转数字
来源：http://hz.zhixingplan.top/gtclpkmiwt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yongpay.top/gtidrrdfqv.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtldkaovku.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtolfykcah.html

[S24] C：获取本地时间
来源：http://hz.nwbrower.top/gtmjowxpas.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gzhubu.top/gtnyeieodl.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtfjuwuuzp.html

memcpy(dst, src, n);
来源：http://hz.aizwys.cn/gtzhpbvukf.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gthytjhwiw.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtlvxstvjq.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtsmbigcwf.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gthbwjvfyo.html

[S28] C：静态变量
来源：http://hz.havefunace.top/gtdroyeest.html

static int counter = 0;
来源：http://hz.sufxvd.cn/gttughlfqy.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gtodducwws.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gtrgnirise.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtqqdikbhz.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtyflmmtbh.html

#define X_H
来源：http://hz.xingfuxueyuan.xyz/gtovmrkeim.html

#endif
来源：http://hz.gotoacloud.top/gtvnytgmvw.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtlorzzgct.html


<!-- 参考信息 -->
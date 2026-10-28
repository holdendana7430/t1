代发 wailian999

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtkrkltdit.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gtxujfnavi.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtzgbqvzqr.html

COMMIT;
来源：http://hz.cqqwz.cn/gtzkhulmvh.html

[Q65] 回滚事务
来源：http://hz.jianghu66.top/gtsquydhcc.html

ROLLBACK;
来源：http://hz.snrcjt.cn/gturxzuzwe.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtyzwrjogv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtnbuynzak.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtkcfrvsyo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtrewvpgab.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtllvhzhdo.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtveqyqsdp.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtxpeuyegx.html

[Q69] 查看执行计划
来源：http://hz.vqdsnc.cn/gtmwjmcgnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtksdmgxvg.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtaaknjrfk.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtcnxzmnph.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtuhdficyc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yongpay.top/gttbecwvot.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtkgcsnlni.html

SHOW INDEX FROM users;
来源：http://hz.hammf.cn/gtkgwlmtzm.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gtauosaozj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jlsjyb.cn/gtovqjnxya.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtnhaqzyhc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtjgsgrmio.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtkvuzstvv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtkqlpphnn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtqbebqmdb.html

[Q76] 按天统计
来源：http://hz.hfpthk.cn/gttfiujivk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtflifubcc.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtvqulgcvr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigfzy.top/gtxtcqyjov.html

[Q78] 当前时间
来源：http://hz.aibaodan.cn/gtkavmdeyz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtrbglozhk.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtwkhfyzow.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenjidiqi.icu/gtnmdaoknn.html

[Q80] 字符串截取
来源：http://hz.cqqwz.cn/gtljjcnoup.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtonccltyv.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtprjyivno.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtmobwcncy.html

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtmgspxfjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtwqmxvouo.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtxueapyjj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ehwqpu.com/gtfbhatpir.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtyohgahoh.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtdnwwpqzm.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtzlizncga.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtilvmtrsi.html

[Q86] 读取 JSON 字段
来源：http://hz.chenzaomai.com/gtwvswskxm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gtvcciqlza.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtqicexhrc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtecatjiuq.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinyuanbaomall.cn/gtncbfhhpn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtmqmocfbc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gtojecelpt.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtbmbrwpvh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtvyixsjcw.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtmhfjgair.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gtavhnadku.html

================================================================================
来源：http://hz.sweek.top/gtgqsvswkc.html

R. Bash 专题
来源：http://hz.dianchejie.cn/gtainegccf.html

================================================================================
来源：http://hz.iojbl.cn/gttdcnvjvs.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtiybwmsre.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtmvvkuwin.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtkosrkius.html

[R02] 变量赋值与使用
来源：http://hz.hammf.cn/gtfrmsmbfb.html

name="Tom"; echo "$name"
来源：http://hz.316326.xyz/gtkjxeytpj.html

[R03] 只读变量
来源：http://hz.pycfn.com/gthdimyoba.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtmcaddjsr.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtcdcopqfa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guowangkeji.top/gtuxezaekd.html

[R05] 参数默认值
来源：http://hz.iojbl.cn/gtxtdhvuer.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtvtgeqjgb.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtdrmklhhq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gttlskaesy.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtdipicqch.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pycfn.com/gtzupwexoz.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtjzvjohew.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtlqisdkro.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtnjprmyln.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtfnyacfyo.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtwdtaoref.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtychtwbbm.html

[R11] case 多分支
来源：http://hz.sweek.top/gtenpceylx.html

case "$1" in
来源：http://hz.jinqigufen.top/gtpdnhqwpo.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtntowryuw.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtvqinipzz.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtoapdrkji.html

esac
来源：http://hz.hnqzz.top/gtoiksfilg.html

[R12] for 遍历文件
来源：http://hz.aibaodan.cn/gtclsupzuv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtjigtrxmb.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtwfikvtct.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtpasoahpr.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtktvnuisa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtddwubxax.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtmbbotvjs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.svipenyu.cn/gtcksvqyml.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtnfvtcafr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gtejkgpjqa.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtpkvltdgu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtbfytvhmb.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtsdoxzdcj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinghuilouyu.cn/gtjctullxc.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gtjbtymawg.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtztieduqg.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtwvglueux.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtonqbarso.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtpwelbnvk.html

echo "${#s}"
来源：http://hz.bjfxy.top/gtfdmdtvov.html

[R22] 截取子串
来源：http://hz.xinyue.icu/gtldrrraml.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangtech.top/gtokfjptbe.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gttlckstpa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtudafidvf.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtdejfxdko.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cucudq.cn/gtchirzprq.html

[R25] 去后缀 / 去前缀
来源：http://hz.birdmap.top/gtfgqhqamp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnqzz.top/gtjlmxyffx.html

[R26] 命令替换
来源：http://hz.ywan-chungtsiang.top/gtuskcpwvd.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gtsdrzuyii.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtpqhxhnhu.html

echo $((1 + 2 * 3))
来源：http://hz.xingfuxueyuan.xyz/gtpyuaxeuw.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtgqqthell.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtuqhjvuxy.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gttdysxgha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtbqzyrubr.html

[R30] 函数返回状态码
来源：http://hz.zhixingplan.top/gtvwkyfyrf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhengqikj.top/gtxemnpllg.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gtzxmtxnhg.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinyuanbaomall.cn/gtcuaaivmh.html

[R32] 参数个数校验
来源：http://hz.316326.xyz/gtyhlpqzem.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtobgwlelj.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtlfthwfih.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgfzy.top/gtvqblbedd.html

[R34] 退出时清理
来源：http://hz.xinyue.icu/gtirfjuusj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtsblkwczx.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtduszdhwl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.vqdsnc.cn/gteftsdhrr.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gtsbtimzrw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.havefunace.top/gteskfasuy.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gttnqtvrbj.html

files=$(ls -1)
来源：http://hz.nwbrower.top/gtydzbzmto.html

[R38] 管道串联
来源：http://hz.pycfn.com/gtmrjnrhzs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydzc1.top/gtetklvaac.html

[R39] 重定向标准输出与错误
来源：http://hz.mhx1999.top/gtepztzkdf.html

cmd > out.log 2>&1
来源：http://hz.fengsongda.top/gtcrzmpqwi.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtgouvywwl.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtmtfemcwa.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gtuxtqfqsv.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtuelbwuku.html

[R42] 输入重定向
来源：http://hz.yonumen.top/gtxmidajyt.html

wc -l < a.txt
来源：http://hz.haohaochexian.top/gtzinsidno.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangkeji.top/gtojmfbnrt.html

find . -name "*.log" -type f
来源：http://hz.quarkkingdee.top/gtdrxvmilv.html

[R44] 按修改时间查找
来源：http://hz.zhongyouzk.top/gtoqamoagn.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtnzocqukr.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtwhfpqjjp.html

find . -name "*.tmp" -delete
来源：http://hz.jianghu66.top/gttzzrkufs.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtttbpjuyg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtobartaxw.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtpkxbigrd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtcthwmafz.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtmiqrszol.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtenzfeqex.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtmudrcuso.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daxiang520.top/gtioeywmsa.html

[R50] awk 求和
来源：http://hz.jinqigufen.top/gtuqarwieq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtvxsyogip.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtmonzmtxy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuxming.cn/gthnprjwuo.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtfnkshkly.html

wc -l a.txt
来源：http://hz.gogol.net.cn/gtbbpjcvza.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gttanmcdtb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtahaybvzf.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gteohrrmdd.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gtegmfpich.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtjbarsbmp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jiagoushi.top/gtsiagxjql.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtrffnejsb.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtkpenwxqt.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtniuixlqf.html

ssh user@host 'uptime'
来源：http://hz.daxiang520.top/gtrgkzvzyq.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtkysnjtmk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gtjqqcpzjx.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtegxoglkr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtnzclirlo.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtjkkhruep.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtfyalaaqm.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtckxnzvpj.html

df -h;  du -sh *
来源：http://hz.jinqigufen.top/gtyuomzzxd.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gtihtypxsn.html

du -ah . | sort -rh | head -10
来源：http://hz.havefunace.top/gtogiawssj.html

[R63] 内存与进程
来源：http://hz.jlsjyb.cn/gtxrmxmuvu.html

free -h;  ps aux | grep nginx
来源：http://hz.xinyue.icu/gtgonaesfz.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtahclsjav.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gotoacloud.top/gtznzhniwy.html

[R65] 查看端口占用
来源：http://hz.cashguo.top/gtumlpyieb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhixingplan.top/gtoefxwnjn.html

[R66] 定时任务
来源：http://hz.tian-w.cn/gtczoolyak.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gtemexuytb.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtniircqhd.html

openssl rand -hex 16
来源：http://hz.zhijiandao.cn/gtprgexwgg.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtdtwagico.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtomvxfgbg.html

[R69] 生成随机密码
来源：http://hz.andypj.xyz/gtwyfunzmk.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtdibzvvbs.html

[R70] 时间戳与互转
来源：http://hz.tianlin.xyz/gtvoinrbhs.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtkqdrspsq.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtcgoeqfxb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtoglfnvdd.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtcmpqcmfo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtkaftsmdf.html

[R73] 分割大日志
来源：http://hz.zhongyouzk.top/gtyrtdfsvq.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gtpclumpvb.html

[R74] 批量重命名
来源：http://hz.zhiwuduotai.top/gtwxgnplno.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtzprficpp.html

[R75] 导出环境变量
来源：http://hz.nwbrower.top/gtvhorpycv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtxcmozpyk.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gtmwldqwgt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gthdtsgwey.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtburrwtny.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gtlzzbnlha.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gtyxkuawff.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtbyzfcdut.html

[R79] 解析命令行选项
来源：http://hz.cheryme.top/gtrkniyoso.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gtwwjoucwx.html

[R80] 查看脚本执行耗时
来源：http://hz.snrcjt.cn/gtauyxukfa.html

time ./run.sh
来源：http://hz.smart0.xyz/gtpunbxvsm.html

================================================================================
来源：http://hz.tanke756.top/gtusowawjs.html

S. C / C++ 专题
来源：http://hz.nanxuanxn.top/gtpswavrye.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmmdtxwoq.html

[S01] C：Hello World
来源：http://hz.shanyushiyangtech.top/gtmqbqjnar.html

#include <stdio.h>
来源：http://hz.tanke756.top/gtawirghoe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuetiantiany.cn/gtahxwsohq.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtifsbdgmb.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtgpmhcaia.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtnrimpana.html

int x; scanf("%d", &x);
来源：http://hz.ydjk.org.cn/gtxnjwrucn.html

[S04] C：字符串复制
来源：http://hz.ppjwa.cn/gtudnsbyrl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yongpay.top/gtwwhukxid.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtdixdtyhw.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtrmmrjcza.html

[S06] C：字符串比较
来源：http://hz.guannengcc.top/gtkalafrfb.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtqxmbbcfd.html

[S07] C：数组遍历求和
来源：http://hz.zhiwuduotai.top/gtljvqsave.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.smart0.xyz/gtfjrjaekd.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtbdiewved.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ybcxt.top/gtziuylnib.html

[S09] C：结构体定义与初始化
来源：http://hz.zdqjudy.top/gtzgnxugqx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shuidangran.top/gtjpkckhgi.html

[S10] C：指针与解引用
来源：http://hz.zhixingplan.top/gtcazxmend.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gtlcapnqjb.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtkxgfbmdr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.svipenyu.cn/gtigeuvtxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtyjxhyxxb.html

fclose(f);
来源：http://hz.sweek.top/gtxgmplsfy.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtuxihrtnh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtdfprurar.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtngqnxpgq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gtauuscfxw.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtnptwqhvs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yanxiufei.cn/gtafxixzzd.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gtdrgmatxc.html

(double) a / b
来源：http://hz.zhixingplan.top/gtksbirdnv.html

[S16] C：位操作置位
来源：http://hz.jiagoushi.top/gtigvrvaue.html

x |= (1 << 3);
来源：http://hz.jianghu66.top/gthrmgzjxr.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtjfykkxpl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gtykszxlca.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gtfussfxon.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtipiutzuu.html

[S19] C：快速排序
来源：http://hz.andypj.xyz/gtlunqbkaj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtuouniluw.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gttiyftonz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtfmkxdukv.html

[S21] C：字符类别判断
来源：http://hz.jiagoushi.top/gtdqeigmcj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gotoacloud.top/gtotonaues.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtnmdvtczs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zycfv.cn/gtymtnddlb.html

[S23] C：随机数
来源：http://hz.tian-w.cn/gtdbhxhcan.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.quarkkingdee.top/gtzadkbaqg.html

[S24] C：获取本地时间
来源：http://hz.yonumen.top/gtxjdjhrdt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtaslddaxy.html

[S25] C：内存拷贝
来源：http://hz.chenlongwang.top/gtmkgzwink.html

memcpy(dst, src, n);
来源：http://hz.jiagoushi.top/gtinpynuhd.html

[S26] C：内存清零
来源：http://hz.shuidangran.top/gtqdidigxz.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtwskuokme.html

[S27] C：定义常量
来源：http://hz.daria6918.cn/gtiuukrzns.html

const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtkkelqmbb.html

[S28] C：静态变量
来源：http://hz.cucudq.cn/gteqshodsh.html

static int counter = 0;
来源：http://hz.meibo888.top/gtqfdnlalz.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtpvczysbj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ehwqpu.com/gtloxhlgvj.html

[S30] C：头文件保护
来源：http://hz.shuidangran.top/gttlhxbclq.html

#ifndef X_H
来源：http://hz.yj202588.top/gtsuyhvmqq.html

#define X_H
来源：http://hz.ehwqpu.com/gtjxyaryqp.html

#endif
来源：http://hz.hnqzz.top/gtfzfvpegk.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtniyoqqrq.html

#include <iostream>
来源：http://hz.xuanzx.com/gtuaqehqgz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtrwskrwku.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtwgyigakg.html

std::string s = "hi";  s += "!";
来源：http://hz.dashuyun.cn/gtnhmklsdn.html


<!-- 参考信息 -->
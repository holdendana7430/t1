代发 wailian999

[Q63] 开启事务
来源：http://hz.9152youxi.cn/gtsctojvms.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtiungxvlw.html

[Q64] 提交事务
来源：http://hz.cqqwz.cn/gtfxmrzvtj.html

COMMIT;
来源：http://hz.svipenyu.cn/gtyrxdjrti.html

[Q65] 回滚事务
来源：http://hz.shuidangran.top/gtonavwwvx.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtmbkjsylj.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtbkjcpkub.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtwptmagpe.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtynkpzddb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.kuanghao11.cn/gtgztujxmy.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtblrffskt.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtmdgoulla.html

ROLLBACK TO sp1;
来源：http://hz.hammf.cn/gtnrlhdpko.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtdqmevnyt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtkobokcea.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtjrjzemui.html

ANALYZE TABLE users;
来源：http://hz.guannengcc.top/gtzldkntxo.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gtyhgkryci.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuxming.cn/gtjnlhdocc.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtaigpnvxe.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtombalblw.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtnfgfwqzg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dianchejie.cn/gtteuaumpx.html

[Q74] 强制使用索引
来源：http://hz.birdmap.top/gtrgnybuid.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangtech.top/gtpjrffllj.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gthzvcpkfb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtwsgtqnrd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtsgqbfpcv.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtfkjiuwuf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuetiantiany.cn/gtgcqzheka.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtybzzppjz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tanke756.top/gthvqrykpr.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtcfljhisd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guannengcc.top/gtwzppzrps.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtvusatsnm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtrfjyhigr.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtimtrbseq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.haohaochexian.top/gtznvhigzz.html

[Q81] 字符串替换
来源：http://hz.andypj.xyz/gtbsjhkjrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtrvguaiau.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gteaxofhid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtmmwhyoud.html

[Q83] 大小写转换
来源：http://hz.jiagoushi.top/gtdqsfosvd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hfpthk.cn/gtznzdtdtd.html

[Q84] 去除首尾空格
来源：http://hz.jyoumei.cn/gtvuzurvke.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtkupbzumg.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gtpjeeiwni.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtdfgeeeys.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtgbydwfnj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dianchejie.cn/gtmcffqjaw.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtwmzfhtou.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.meibo888.top/gtcphaskym.html

[Q88] 行转列（条件聚合）
来源：http://hz.cqqwz.cn/gtomnqkuje.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtljrdoitt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtvhqnwcet.html

[Q89] 判断表是否存在
来源：http://hz.ybcxt.top/gtsllhzddz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj202588.top/gtkokkdwps.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtodksektz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtazkxwekp.html

================================================================================
来源：http://hz.fengsongda.top/gtjilimbna.html

R. Bash 专题
来源：http://hz.pengpengdd.cyou/gtcoaqrech.html

================================================================================
来源：http://hz.sufxvd.cn/gtnltnceky.html

[R01] shebang 与严格模式
来源：http://hz.dianchejie.cn/gtzrqokzyc.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtfmedactl.html

set -euo pipefail
来源：http://hz.jqgufenzy.top/gtjgifyrvk.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtreqlpapt.html

name="Tom"; echo "$name"
来源：http://hz.jinghuilouyu.cn/gtbjrheomp.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtxuahjvjv.html

readonly PI=3.14
来源：http://hz.zhoulong.xyz/gtrahghcbg.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtjcepgtac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtharxsodc.html

[R05] 参数默认值
来源：http://hz.cdnleiting.top/gtjpwudihl.html

name="${1:-default}"
来源：http://hz.yj202588.top/gtcecueqkt.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtnlwzpcpo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sysykeji.top/gtfduerdpi.html

[R07] if 判断文件
来源：http://hz.svipenyu.cn/gtypjojuwy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daria6918.cn/gtdjhgqfrm.html

[R08] 数值比较
来源：http://hz.daxiang520.top/gtelgweoch.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtwlblvjvu.html

[R09] 字符串比较
来源：http://hz.jyoumei.cn/gtyuqqtqjz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258.top/gtzxeaamuk.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtmsvuzalq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gtaknltsvb.html

[R11] case 多分支
来源：http://hz.redwolf501.top/gtcresghzq.html

case "$1" in
来源：http://hz.ydzc1.top/gtkfwmlsgu.html

start) echo "启动" ;;
来源：http://hz.iojbl.cn/gttxznraof.html

stop)  echo "停止" ;;
来源：http://hz.zhongyouzk.top/gtmrwzpkmd.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtlrqarbuc.html

esac
来源：http://hz.nwbrower.top/gtwvbrhral.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtuecwwcsr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.0kj1m.cn/gtqtxlvqov.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtzixsjmst.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtxlvnrnnx.html

[R14] C 风格 for
来源：http://hz.zhongyouzk.top/gtmkhlysxs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtxefyduci.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtioxpwjur.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtvommdovf.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtcxjwefnq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtlcgmbsug.html

[R17] 数组定义与取值
来源：http://hz.zhoulong.xyz/gthflprrqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yangfankeji.com/gturirvqti.html

[R18] 遍历数组
来源：http://hz.gogol.net.cn/gtlicusrwj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtseajazzb.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtkjtkflvr.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtfvokgmaf.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gttzjdpdak.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gtpkfitelu.html

[R21] 字符串长度
来源：http://hz.jianghu66.top/gtztzrzflz.html

echo "${#s}"
来源：http://hz.nwbrower.top/gtnoqsuruz.html

[R22] 截取子串
来源：http://hz.tanke756.top/gtgloocknd.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtrjgtucjz.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtejclyzqz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.quarkkingdee.top/gtamulivaj.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gtyqaldvmu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangshuangyany.cn/gtoyzvbqdb.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtajitoflj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtemrklftd.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtwzpyvidq.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtinhdmeub.html

[R27] 算术展开
来源：http://hz.chenlongwang.top/gtpqgcizft.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtoqtiylit.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtuidirgfu.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtjomkwesc.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtzclvbbne.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtcztwesbc.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtxklxbbmm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gthfuvhlry.html

[R31] 局部变量
来源：http://hz.ydzc1.top/gtnrodswms.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtpqevvoac.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtyzmejfww.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.kuanghao11.cn/gtgdqksoir.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtbuylwlly.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.andypj.xyz/gtddboglal.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtjogqlphc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtlxwgbxub.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtmruxoowe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gzhubu.top/gthulkuszm.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gtbjzphaaw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gthmywzohz.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtyyfhfkyi.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtcegvuhga.html

[R38] 管道串联
来源：http://hz.hnxiangtu.top/gteklcrgrs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.quarkkingdee.top/gtdfordgcj.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtgaeeipnj.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtaaaclqtc.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtlcpzmtfr.html

echo "log" >> out.log
来源：http://hz.jqgfzy.top/gtuaoxenwc.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gthdnbcsub.html

cmd >/dev/null 2>&1
来源：http://hz.aizwys.cn/gtkovykifj.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtkglpgcug.html

wc -l < a.txt
来源：http://hz.meibo888.top/gteiqqtmeb.html

[R43] 按名字查找文件
来源：http://hz.jinyuanbaomall.cn/gtoyfzpilk.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtkbwyswqh.html

[R44] 按修改时间查找
来源：http://hz.ivvv.top/gtnstxdspw.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtepxvzwci.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtfsgsezbl.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtshyzmvqo.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtprlawspr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.kuanghao11.cn/gtklxunmdj.html

[R47] sed 单行替换
来源：http://hz.jinqigufen.top/gtluxvzwtd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gaohongyu789.top/gtxktlnowo.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtvxgixgny.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhiwuduotai.top/gtyuxfsxfs.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtgvgdgzsa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenlongwang.top/gtegzvzzjv.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gttuuckswe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fzhhl.top/gtzqzjjxjh.html

[R51] 排序去重取前几
来源：http://hz.bjfxy.top/gtzadclxod.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gtoirqrpfs.html

[R52] 统计行数
来源：http://hz.gotoacloud.top/gtbsaadgri.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtmovbftzn.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtkzggqoem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgfzy.top/gtonwjlxcn.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtjycycwwj.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtgllplprw.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtijryfaut.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtusdepiqm.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtujyzobds.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtpprjwlho.html

[R57] 远程执行命令
来源：http://hz.zhiwuduotai.top/gtuemsrucc.html

ssh user@host 'uptime'
来源：http://hz.nanxuanxn.top/gtayayrrpc.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtsxgunelg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.birdmap.top/gtibebarlh.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtrrryzruu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hfpthk.cn/gtcsgmskqk.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtlxcoyeax.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhixingplan.top/gtrmvggtpo.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtzvbfbyni.html

df -h;  du -sh *
来源：http://hz.ehwqpu.com/gtzkardgdr.html

[R62] 找最占空间的文件
来源：http://hz.yangfankeji.com/gtfqsgquze.html

du -ah . | sort -rh | head -10
来源：http://hz.pycfn.com/gttjsdsvmj.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtcexsmvas.html

free -h;  ps aux | grep nginx
来源：http://hz.smart0.xyz/gtyuncogtd.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtbxrmgflv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gttbensnkz.html

[R65] 查看端口占用
来源：http://hz.yangfankeji.com/gtefsznjzl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gtvgqubpaj.html

[R66] 定时任务
来源：http://hz.fzhhl.top/gthfgbthdn.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtpxsxtvbh.html

[R67] 生成随机十六进制串
来源：http://hz.sysykeji.top/gtvanhndvq.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtnaftefnk.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gtifklrwiw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.redwolf501.top/gtwgukamir.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtyomsqgsz.html

head -c 16 /dev/urandom | base64
来源：http://hz.9152youxi.cn/gtlxhfdjyn.html

[R70] 时间戳与互转
来源：http://hz.tian-w.cn/gtmmeceehx.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gthhmtuska.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gtexxnjpqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ppjwa.cn/gtqlsihqfi.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtddzxuziv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtigoneams.html

[R73] 分割大日志
来源：http://hz.haohaochexian.top/gtdrczmlxw.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gtytxpcvme.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtzofqiktu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtunbkzssu.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtjeupzihb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sxryk.cn/gtetrdkupa.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtrtjgeuyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gteemwzowo.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtratckhnc.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gthgodpxwt.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gtywgeobrd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pycfn.com/gtzbbuqpoe.html

[R79] 解析命令行选项
来源：http://hz.zdqjudy.top/gtqkzmpjtg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtwfyrmsbe.html

[R80] 查看脚本执行耗时
来源：http://hz.iojbl.cn/gtnnkrhpkl.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtfqnnxrnl.html

================================================================================
来源：http://hz.52xcode.cn/gtubxgprol.html

S. C / C++ 专题
来源：http://hz.bjfxy.top/gtlsubdmog.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgkbmhtfs.html

[S01] C：Hello World
来源：http://hz.zycfv.cn/gttlitikeq.html

#include <stdio.h>
来源：http://hz.xuetiantiany.cn/gtjmbzujgh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtlemvxhqs.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtggdivsqz.html

int a = 10; printf("%d\n", a);
来源：http://hz.yangfankeji.com/gtoirnodwp.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtncyotemm.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtcprbebzd.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtmgwyjtsu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.birdmap.top/gtibdtkyhr.html

[S05] C：字符串长度
来源：http://hz.pengpengdd.cyou/gtweiyemsj.html

strlen(s)
来源：http://hz.gogol.net.cn/gtbowyyzkx.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtrgzypcng.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtkzzxyewj.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtofpiwith.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtvslyowtw.html

[S08] C：动态内存分配与释放
来源：http://hz.316326.xyz/gtjeyxkcvj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtsmehivaq.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtuvhitlca.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtptqqneec.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtccjqecxo.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtutvngyuz.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtwnweucbq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jianghu66.top/gtmqcgzlex.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgfzy.top/gtanodtzuj.html

fclose(f);
来源：http://hz.yongpay.top/gtowznxccd.html

[S12] C：写文件
来源：http://hz.yj20258888.top/gtbeglrhcr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtjxipyinz.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtzniotsxe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtaosdbfba.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtcpupomsf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gtgvqcostw.html

[S15] C：类型转换
来源：http://hz.cashguo.top/gteanvztds.html

(double) a / b
来源：http://hz.yangfankeji.com/gtewnanxeq.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtnesubmog.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gtramtymqw.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtvfyfnees.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtmnexalkr.html

[S18] C：命令行参数
来源：http://hz.yj20258.top/gtfcjntuli.html

int main(int argc, char **argv)
来源：http://hz.mhx1999.top/gtzggfjnuo.html

[S19] C：快速排序
来源：http://hz.quarkkingdee.top/gtqzewugml.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtqgnqakpq.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtnhsyxrcx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gthpjggvvq.html

[S21] C：字符类别判断
来源：http://hz.fzhhl.top/gtjnxuqitq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtidrekyil.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtozsswhls.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gtyffzsnqw.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtnwalzjhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yanxiufei.cn/gtunzquhnf.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtbpovyamr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhengqikj.top/gtbikeswso.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtsnxrrpng.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gttewqddiz.html

[S26] C：内存清零
来源：http://hz.guannengcc.top/gtcsggbkex.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtkawfwjcs.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtgiojrrjg.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtfstxsgcm.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtbjfrzugc.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtwatqnmdd.html

[S29] C：变参函数
来源：http://hz.52xcode.cn/gtncixqwxr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtohphruho.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtpjpettib.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtawvdzkeb.html

#define X_H
来源：http://hz.hfpthk.cn/gtcusmvxrq.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtruakvkqh.html

[S31] C++：Hello World
来源：http://hz.xuetiantiany.cn/gtrsitjnns.html

#include <iostream>
来源：http://hz.zdqjudy.top/gtcfytyyoi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.smart0.xyz/gtqngjzgug.html

[S32] C++：字符串
来源：http://hz.hfpthk.cn/gtusqeoehe.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtnlzzvddk.html


<!-- 参考信息 -->